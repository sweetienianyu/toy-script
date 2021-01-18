## A mini parser

```
// do 构造器表示按顺序执行多个操作
// 不同操作同逗号分割
do(define(x, 10),
  if(>(x, 5),
    print("large"),
    print("small")))
```

```
// 解析用于描述程序的数据结构由表达式对象组成，每个表达式对象都有一个type属性 来指示它的表达式类型以及描述其内容的其他属性
// value类型：字符串或者数字 有value属性
// word类型: 标识符名称  有name属性
// apply类型: 应用表达式 有operator属性 有包含参数的arg属性
```