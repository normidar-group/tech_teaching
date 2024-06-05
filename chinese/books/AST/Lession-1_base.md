# AST的基础

AST是一种树的结构，用来解释编程语言，也就是解释逻辑。

在编程语言中通常存在这样的树：

```tree
Statement
├── Expression
└── Type
```

用面向对象的说法来说就是：【所有东西都是Statement】

假设我们有几行的代码例如：

```dart
int sum = 0;
for (int i = 0; i < 100; i++) {
    sum = sum + i;
}
```

那我们的AST将会像是这样：

```yaml
Codes:
 - CodeType: Define
   Type: Int
   Name: sum
   Exp: 0
 - CodeType: ForLoop
   Define: "int i = 0"
   Condition: "i < 100"
   Step: "i++"
   Body:
    - CodeType: Assign
      Target: sum
      Exp:
       - CodeType: Addition
         Left: sum
         Right: i
```

使用JSON来表现就是这样：

```json
{
  "Codes": [
    {
      "CodeType": "Define",
      "Type": "Int",
      "Name": "sum",
      "Exp": 0
    },
    {
      "CodeType": "ForLoop",
      "Define": "int i = 0",
      "Condition": "i < 100",
      "Step": "i++",
      "Body": [
        {
          "CodeType": "Assign",
          "Target": "sum",
          "Exp": [
            {
              "CodeType": "Addition",
              "Left": "sum",
              "Right": "i"
            }
          ]
        }
      ]
    }
  ]
}
```

> AST仅供参考

AST的目的是拆分语言为对象以供进一步的处理。在上面我们可以看到整个代码包含在一个Code中的列表中，这表示整体代码在AST看来是一个列表。再看向`ForLoop -> Body` 我们也发现一个列表在其中，这是因为`{...}`中所存放的是代码块代码块就是代码行的列表。
