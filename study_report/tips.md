
println!("hello") rust语言中的 宏 都以！号结尾

#变量：
- 基本数据类型：整型、浮点型、布尔类型、字符类型

- rust会自动从等号右边推断出变量的类型
```let 变量名=值； 不指定变量类型
let food="螃蟹";
let score=99;
let checked=true;
println!("food is {}",food);```

- 命名：
1.必须以字母、下划线开头，不能以数字开头
2.要区分大小写

- 整型：
有符号类型：i
无符号类型：u

- 浮点型：
1. 按照存储大小，把浮点型划分为单精度 f32 和双精度 f64（默认的浮点类型）
2. Rust 中不能将 0.0 （浮点数）赋值给任意一个整型，也不能将 0 （整数）赋值给任意一个浮点型，会报错，如：```let price8:f64 = 99;```
```
let price9 = 18.00;        // 默认是 f64
let price10:f32 = 8.88;
let price11:f64 = 168.125;  // 双精度浮点型```

println!("price9 {}", price9); //输出 price9 18
println!("price10 {}", price10);//输出 price10 8.88
println!("price11 {}", price11);//输出 price11 168.125

- 字符（char)：
1. 字符串的基本组成部分，也就是单个字符或字。字符数据类型 包含了 数字、字母、Unicode 和 其它特殊字符。
2. ```let c:char='R';```
3. 注：Rust 的字符只能用 '' 来表示， "" 是留给字符串的
4. Rust 使用 UTF-8 作为底层的编码 ，而不是常见的使用 ASCII 作为底层编码。

- 字符串


- 布尔：
1. ```let checked:bool = true;
println!("checked {}", checked);//输出 checked true```




- 元组：
```let tuple变量名称：(数据类型1，数据类型2...)=(数据1，数据2）```
```let tuple变量名称=（数据1，数据2.。```

- 所有权：

放在栈上：因为是后进先出，所以类型大小是固定的，如i32
放在堆上：编译时大小不确定 用户自己管理



