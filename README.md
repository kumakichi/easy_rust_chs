## 更新

![example workflow name](https://github.com/kumakichi/easy_rust_chs/workflows/github%20pages/badge.svg)

2021年2月1日: [Youtube视频](https://www.youtube.com/playlist?list=PLfllocyHVgsRwLkTAhG0E-2QxCf-ozBkk)

2021年1月4日: 支持在线查看 [点击阅读](https://kumakichi.github.io/easy_rust_chs)

## 介绍

Rust是一种新的语言，已经有了很好的教科书。但是有时候它的教材很难，因为它的教材是给以英语为母语的人看的。现在很多公司和人学习Rust，如果有一本英语简单的书，他们可以学得更快。这本教材就是给这些公司和人用简单的英语来学习Rust的。

Rust是一门很新的语言，但已经非常流行。它之所以受欢迎，是因为它给你提供了C或C++的速度和控制力，但也给你提供了Python等其他较新语言的内存安全。它用一些新的想法来实现这一点，这些想法有时与其他语言不同。这意味着有一些新的东西需要学习，你不能只是 "边走边想"。Rust是一门语言，你必须思考一段时间才能理解。但如果你懂其他语言的话，它看起来还是很熟悉的，它是为了帮助你写好代码而生的。

## 我是谁？

我是一个生活在韩国的加拿大人，我在写Easy Rust的同时，也在思考如何让这里的公司开始使用它。我希望其他不以英语为第一语言的国家也能使用它。

## 简单英语学Rust

*简单英语学Rust*写于2020年7月至8月，长达400多页。如果你有任何问题，可以在这里或[在LinkedIn上](https://www.linkedin.com/in/davemacleod)或[在Twitter上](https://twitter.com/mithridates)联系我。如果你发现有什么不对的地方，或者要提出pull request，请继续。已经有超过20人帮助我们修复了代码中的错别字和问题，所以你也可以。我不是世界上最好的Rust专家，所以我总是喜欢听到新的想法，或者看看哪里可以让这本书变得更好。

- [第1部分 - 浏览器中的Rust](#第1部分---浏览器中的Rust)
  - [Rust Playground](#rust-playground)
  - [🚧 and ⚠️](#和%EF%B8%8F)
  - [注释](#注释)
  - [类型](#类型)
    - [原始类型](#原始类型)
  - [类型推导](#类型推导)
    - [浮点数](#浮点数)
  - [打印hello, world!](#打印hello-world)
    - [声明变量和代码块](#声明变量和代码块)
  - [显示和调试](#显示和调试)
    - [最小和最大的数](#最小和最大的数)
  - [可变性](#可变性)
    - [遮蔽](#遮蔽)
  - [栈，堆和指针](#栈堆和指针)
  - [关于打印的更多信息](#关于打印的更多信息)
  - [字符串](#字符串)
  - [const和static](#const和static)
  - [关于引用的更多信息](#关于引用的更多信息)
  - [可变引用](#可变引用)
    - [再谈shadowing](#再谈shadowing)
  - [函数的引用](#函数的引用)
  - [拷贝类型](#拷贝类型)
    - [无值变量](#无值变量)
  - [集合类型](#集合类型)
    - [数组](#数组)
  - [向量](#向量)
  - [元组](#元组)
  - [控制流](#控制流)
  - [结构体](#结构体)
  - [枚举](#枚举)
    - [使用多种类型的枚举](#使用多种类型的枚举)
  - [循环](#循环)
  - [实现结构和枚举](#实现结构和枚举)
  - [解构](#解构)
  - [引用和点运算符](#引用和点运算符)
  - [泛型](#泛型)
  - [选项和结果](#选项和结果)
    - [选项](#选项)
    - [结果](#结果)
  - [其他集合类型](#其他集合类型)
    - [HashMap和BTreeMap](#HashMap和BTreeMap)
    - [HashSet和BTreeSet](#hashset和btreeset)
    - [二叉堆](#二叉堆)
    - [VecDeque](#vecdeque)
  - [?操作符](#操作符)
    - [When panic and unwrap are good](#when-panic-and-unwrap-are-good)
  - [trait](#trait)
    - [From trait](#from-trait)
    - [在函数中使用字符串和&str](#在函数中使用字符串和&str)
  - [链式方法](#链式方法)
  - [迭代器](#迭代器)
    - [迭代器如何工作](#迭代器如何工作)
  - [闭包](#闭包)
    - [闭包中的_](#闭包中的_)
    - [闭包和迭代器的有用方法](#闭包和迭代器的有用方法)
  - [dbg! 宏和.检查器](#dbg宏和inspect)
  - [&str的类型](#str的类型)
  - [生命期](#生命期)
  - [内部可变性](#内部可变性)
    - [Cell](#cell)
    - [RefCell](#refcell)
    - [Mutex](#mutex)
    - [RwLock](#rwlock)
  - [Cow](#cow)
  - [类型别名](#类型别名)
    - [在函数中导入和重命名](#在函数中导入和重命名)
  - [todo!宏](#todo宏)
  - [Rc](#rc)
  - [多线程](#多线程)
  - [函数中的闭包](#函数中的闭包)
  - [impl Trait](#impl-trait)
  - [Arc](#arc)
  - [Channels](#channels)
  - [阅读Rust文档](#阅读Rust文档)
    - [assert_eq! ](#assert_eq)
    - [搜索](#搜索)
    - [[src]按钮](#src-按钮)
    - [trait信息](#trait信息)
  - [属性](#属性)
  - [Box](#box)
  - [Box around traits](#box-around-traits)
  - [默认值和建造者模式](#默认值和建造者模式)
  - [Deref和DerefMut](#Deref和DerefMut)
  - [Crate和模块](#Crate和模块)
  - [测试](#测试)
    - [测试驱动的开发](#测试驱动的开发)
  - [外部crate](#外部crate)
    - [rand](#rand)
    - [rayon](#rayon)
    - [serde](#serde)
    - [regex](#regex)
    - [chrono](#chrono)
  - [标准库之旅](#标准库之旅)
    - [数组](#数组-1)
    - [char](#char)
    - [Integer](#integers)
    - [Floats](#floats)
    - [Bool](#bool)
    - [Vec](#vec)
    - [String](#string)
    - [OsString和CString](#OsString和CString)
    - [Mem](#mem)
    - [Prelude](#prelude)
    - [Time](#time)
    - [其他宏](#其他宏)
    - [编写宏](#编写宏)
- [第2部分 - 电脑上的Rust](#第2部分---电脑上的Rust)
  - [cargo](#cargo)
  - [接受用户输入](#接受用户输入)
  - [使用文件](#使用文件)
  - [cargo文档](#cargo文档)
  - [结束了吗？](#结束了吗？)

# 第1部分 - 浏览器中的Rust

本书有两个部分。第1部分，你将在浏览器中就能学到尽可能多的Rust知识。实际上你几乎可以在不安装Rust的情况下学到所有你需要知道的东西，所以第1部分非常长。最后是第二部分。它要短得多，是关于电脑上的Rust。在这里，你将学习到其他一切你需要知道的、只能在浏览器之外进行的事情。例如:处理文件、接受用户输入、图形和个人设置。希望在第一部分结束时，你会喜欢Rust，以至于你会安装它。如果你不喜欢，也没问题--第一部分教了你很多，你不会介意的。

## Rust Playground

也许你还不想安装Rust，这也没关系。你可以去[https://play.rust-lang.org/](https://play.rust-lang.org/)，在不离开浏览器的情况下开始写Rust。你可以在那里写下你的代码，然后点击Run来查看结果。你可以在浏览器的Playground里面运行本书中的大部分示例。只有在接近结尾的时候，你才会看到无法在Playground运行的示例(比如打开文件)。

以下是使用Rust Playground时的一些提示。

- 用"Run"来运行你的代码

- 如果你想让你的代码更快，就把Debug改为Release。Debug:编译速度更快，运行速度更慢，包含调试信息。Release:编译速度更慢，运行速度更快，删除调试信息。
- 点击Share，得到一个网址链接，你可以用它来分享你的代码。如果你需要帮助，可以用它来分享你的代码。点击分享后，你可以点击`Open a new thread in the Rust user forum`，马上向那里的人寻求帮助。
- Rustfmt工具: Rustfmt会很好地格式化你的代码。
- TOOLS: Rustfmt会很好地格式化你的代码。Clippy会给你额外的信息，告诉你如何让你的代码更好。
- CONFIG: 在这里你可以把你的主题改成黑暗模式，这样你就可以在晚上工作了，还有很多其他配置。

如果你想安装Rust，请到这里[https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install)，然后按照说明操作。通常你会使用`rustup`来安装和更新Rust。

## 🚧和⚠️

有时书中的代码例子不能用。如果一个例子不工作，它将会有一个🚧或⚠️在里面。🚧就像 "正在建设中"一样:它意味着代码不完整。Rust需要一个`fn main()`(一个主函数)来运行，但有时我们只是想看一些小的代码，所以它不会有`fn main()`。这些例子是正确的，但需要一个`fn main()`让你运行。而有些代码示例向你展示了一个问题，我们将解决这个问题。那些可能有一个`fn main()`，但会产生一个错误，所以它们会有一个⚠️。

## 注释

注释是给程序员看的，而不是给电脑看的。写注释是为了帮助别人理解你的代码。 这也有利于帮助你以后理解你的代码。 (很多人写了很好的代码，但后来却忘记了他们为什么要写它。)在Rust中写注释，你通常使用 `//`．

```rust
fn main() {
    // Rust programs start with fn main()
    // You put the code inside a block. It starts with { and ends with }
    let some_number = 100; // We can write as much as we want here and the compiler won't look at it
}
```

当你这样做时，编译器不会看`//`右边的任何东西。

还有一种注释，你用`/*`开始写，`*/`结束写。这个写在你的代码中间很有用。

```rust
fn main() {
    let some_number/*: i16*/ = 100;
}
```

对编译器来说，`let some_number/*: i16*/ = 100;`看起来像`let some_number = 100;`。

`/* */`形式对于超过一行的非常长的注释也很有用。在这个例子中，你可以看到你需要为每一行写`//`。但是如果您输入 `/*`，它不会停止，直到您用 `*/` 完成它。

```rust
fn main() {
    let some_number = 100; /* Let me tell you
    a little about this number.
    It's 100, which is my favourite number.
    It's called some_number but actually I think that... */

    let some_number = 100; // Let me tell you
    // a little about this number.
    // It's 100, which is my favourite number.
    // It's called some_number but actually I think that...
}
```

## 类型

Rust有很多类型，让你可以处理数字、字符等。有些类型很简单，有些类型比较复杂，你甚至可以创建自己的类型。

### 原始类型

Rust有简单的类型，这些类型被称为**原始类型**(原始=非常基本)。我们将从整数和`char`(字符)开始。整数是没有小数点的整数。整数有两种类型。

- 有符号的整数
- 无符号整数

符号是指`+`(加号)和`-`(减号)，所以有符号的整数可以是正数，也可以是负数(如+8，-8)。但无符号整数只能是正数，因为它们没有符号。

有符号的整数是 `i8`, `i16`, `i32`, `i64`, `i128`, 和 `isize`。

无符号的整数是 `u8`, `u16`, `u32`, `u64`, `u128`, 和 `usize`。

i或u后面的数字表示该数字的位数，所以位数多的数字可以大一些。8位=一个字节，所以`i8`是一个字节，`i64`是8个字节，以此类推。尺寸较大的数字类型可以容纳更大的数字。例如，`u8`最多可以容纳255，但`u16`最多可以容纳65535。而`u128`最多可以容纳340282366920938463463374607431768211455。

那么什么是`isize`和`usize`呢？这表示你电脑的位数。(你的电脑上的位数叫做你电脑的**架构**)。所以32位计算机上的`isize`和`usize`就像`i32`和`u32`，64位计算机上的`isize`和`usize`就像`i64`和`u64`。

整数类型不同的原因有很多。其中一个原因是计算机性能:较小的字节数处理速度更快。例如，数字-10作为`i8`是`11110110`，但作为`i128`是`11111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111110110`。但这里还有一些其他用法。

Rust中的字符叫做`char`. 每一个`char`都有一个数字:字母`A`是数字65，而字符`友`(中文的 "朋友")是数字21451。这个数字列表被称为 "Unicode"。Unicode对使用较多的字符使用较小的数字，如A到Z，或0到9的数字，或空格。

```rust
fn main() {
    let first_letter = 'A';
    let space = ' '; // A space inside ' ' is also a char
    let other_language_char = 'Ꮔ'; // Thanks to Unicode, other languages like Cherokee display just fine too
    let cat_face = '😺'; // Emojis are chars too
}
```

使用最多的字符的数字小于256，它们可以装进`u8`。记住，`u8`是0加上255以内的所有数字，总共256个。这意味着 Rust 可以使用 `as` 将 `u8` 安全地 **cast**成 `char`。("把 `u8` cast成 `char`"意味着 "把 `u8` 假装成 `char`")

用 `as` cast是有用的，因为 Rust 是非常严格的。它总是需要知道类型。
 而不会让你同时使用两种不同的类型，即使它们都是整数。例如，这将无法工作:

```rust
fn main() { // main() is where Rust programs start to run. Code goes inside {} (curly brackets)

    let my_number = 100; // We didn't write a type of integer,
                         // so Rust chooses i32. Rust always
                         // chooses i32 for integers if you don't
                         // tell it to use a different type

    println!("{}", my_number as char); // ⚠️
}
```

原因是这样的:

```text
error[E0604]: only `u8` can be cast as `char`, not `i32`
 --> src\main.rs:3:20
  |
3 |     println!("{}", my_number as char);
  |                    ^^^^^^^^^^^^^^^^^
```

幸运的是，我们可以用`as`轻松解决这个问题。我们不能把`i32`转成`char`，但我们可以把`i32`转成`u8`，然后把`u8`转换成`char`。所以在一行中，我们使用 `as` 将 my_number 变为 `u8`，再将其变为 `char`。现在可以编译了。

```rust
fn main() {
    let my_number = 100;
    println!("{}", my_number as u8 as char);
}
```

它打印的是`d`，因为那是100对应的`char`。

然而，更简单的方法是告诉 Rust `my_number` 是 `u8`。下面是你的做法。

```rust
fn main() {
    let my_number: u8 = 100; //  change my_number to my_number: u8
    println!("{}", my_number as char);
}
```

所以这就是Rust中所有不同数字类型的两个原因。这里还有一个原因:`usize`是Rust用于*索引*的大小。(索引的意思是 "哪项是第一"，"哪项是第二"等等)`usize`是索引的最佳大小，因为:

- 索引不能是负数，所以它需要是一个带u的数字
- 它应该是大的，因为有时你需要索引很多东西，但。
- 不可能是u64，因为32位电脑不能使用u64。

所以Rust使用了`usize`，这样你的计算机就可以得到它能读到的最大的数字进行索引。



我们再来了解一下`char`。你看到`char`总是一个字符，并且使用`''`而不是`""`。

所有的 `字符` 都使用4个字节的内存，因为4个字节足以容纳任何种类的字符:
- 基本字母和符号通常需要4个字节中的1个：`a b 1 2 + - = $ @`
- 其他字母，如德语的 Umlauts 或重音，需要4个字节中的2个： `ä ö ü ß è é à ñ`
- 韩文、日文或中文字符需要3或4个字节： `国 안 녕`

当使用字符作为字符串的一部分时，字符串被编码以使用每个字符所需的最小内存量。

我们可以用`.len()`来看一下。

```rust
fn main() {
    println!("Size of a char: {}", std::mem::size_of::<char>()); // 4 bytes
    println!("Size of string containing 'a': {}", "a".len()); // .len() gives the size of the string in bytes
    println!("Size of string containing 'ß': {}", "ß".len());
    println!("Size of string containing '国': {}", "国".len());
    println!("Size of string containing '𓅱': {}", "𓅱".len());
}
```

这样打印出来。

```text
Size of a char: 4
Size of string containing 'a': 1
Size of string containing 'ß': 2
Size of string containing '国': 3
Size of string containing '𓅱': 4
```

可以看到，`a`是一个字节，德文的`ß`是两个字节，日文的`国`是三个字节，古埃及的`𓅱`是4个字节。

```rust
fn main() {
    let slice = "Hello!";
    println!("Slice is {} bytes.", slice.len());
    let slice2 = "안녕!"; // Korean for "hi"
    println!("Slice2 is {} bytes.", slice2.len());
}
```

这个打印:

```text
Slice is 6 bytes.
Slice2 is 7 bytes.
```

`slice`的长度是6个字符，6个字节，但`slice2`的长度是3个字符，7个字节。

如果`.len()`给出的是以字节为单位的大小，那么以字符为单位的大小呢？这些方法我们后面会学习，但你只要记住`.chars().count()`就可以了。`.chars().count()` 将你写的东西变成字符，然后计算有多少个字符。


```rust
fn main() {
    let slice = "Hello!";
    println!("Slice is {} bytes and also {} characters.", slice.len(), slice.chars().count());
    let slice2 = "안녕!";
    println!("Slice2 is {} bytes but only {} characters.", slice2.len(), slice2.chars().count());
}
```

这就打印出来了。

```text
Slice is 6 bytes and also 6 characters.
Slice2 is 7 bytes but only 3 characters.
```

## 类型推导

类型推导的意思是，如果你不告诉编译器类型，但它可以自己决定，它就会决定。编译器总是需要知道变量的类型，但你并不总是需要告诉它。实际上，通常你不需要告诉它。例如，对于`let my_number = 8`，`my_number`将是一个`i32`。这是因为如果你不告诉它，编译器会选择i32作为整数。但是如果你说`let my_number: u8 = 8`，它就会把`my_number`变成`u8`，因为你告诉它`u8`。

通常编译器都能猜到。但有时你需要告诉它，原因有两个。

1) 你正在做一些非常复杂的事情，而编译器不知道你想要的类型。
2) 你想要一个不同的类型(例如，你想要一个`i128`，而不是`i32`)。

要指定一个类型，请在变量名后添加一个冒号。

```rust
fn main() {
    let small_number: u8 = 10;
}
```

对于数字，你可以在数字后面加上类型。你不需要空格--只需要在数字后面直接输入。

```rust
fn main() {
    let small_number = 10u8; // 10u8 = 10 of type u8
}
```

如果你想让数字便于阅读，也可以加上`_`。

```rust
fn main() {
    let small_number = 10_u8; // This is easier to read
    let big_number = 100_000_000_i32; // 100 million is easy to read with _
}
```

`_`不会改变数字。它只是为了让你方便阅读。而且你用多少个`_`都没有关系。

```rust
fn main() {
    let number = 0________u8;
    let number2 = 1___6______2____4______i32;
    println!("{}, {}", number, number2);
}
```

这样打印出的是`0, 1624`。

### 浮点数

浮点数是带有小数点的数字。5.5是一个浮点数，6是一个整数。5.0也是一个浮点数，甚至5.也是一个浮点数。

```rust
fn main() {
    let my_float = 5.; // Rust sees . and knows that it is a float
}
```

但类型不叫`float`，叫`f32`和`f64`。这和整数一样:`f`后面的数字显示的是位数。如果你不写类型，Rust会选择`f64`。

当然，只有同一类型的浮点数可以一起使用。所以你不能把`f32`加到`f64`上。

```rust
fn main() {
    let my_float: f64 = 5.0; // This is an f64
    let my_other_float: f32 = 8.5; // This is an f32

    let third_float = my_float + my_other_float; // ⚠️
}
```

当你尝试运行这个时，Rust会说。

```text
error[E0308]: mismatched types
 --> src\main.rs:5:34
  |
5 |     let third_float = my_float + my_other_float;
  |                                  ^^^^^^^^^^^^^^ expected `f64`, found `f32`
```

当你使用错误的类型时，编译器会写 "expected (type), found (type)"。它这样读取你的代码。

```rust
fn main() {
    let my_float: f64 = 5.0; // The compiler sees an f64
    let my_other_float: f32 = 8.5; // The compiler sees an f32. It is a different type.
    let third_float = my_float + // You want to add my_float to something, so it must be an f64 plus another f64. Now it expects an f64...
    let third_float = my_float + my_other_float;  // ⚠️ but it found an f32. It can't add them.
}
```

所以，当你看到 "expected(type)，found(type)"时，你必须找到为什么编译器预期的是不同的类型。

当然，用简单的数字很容易解决。你可以用`as`把`f32`转成`f64`。

```rust
fn main() {
    let my_float: f64 = 5.0;
    let my_other_float: f32 = 8.5;

    let third_float = my_float + my_other_float as f64; // my_other_float as f64 = use my_other_float like an f64
}
```

或者更简单，去掉类型声明。("声明一个类型"="告诉Rust使用该类型")Rust会选择可以加在一起的类型。

```rust
fn main() {
    let my_float = 5.0; // Rust will choose f64
    let my_other_float = 8.5; // Here again it will choose f64

    let third_float = my_float + my_other_float;
}
```

Rust编译器很聪明，如果你需要f32，就不会选择f64。

```rust
fn main() {
    let my_float: f32 = 5.0;
    let my_other_float = 8.5; // Usually Rust would choose f64,

    let third_float = my_float + my_other_float; // but now it knows that you need to add it to an f32. So it chooses f32 for my_other_float too
}
```

## 打印hello, world!

当你启动一个新的Rust程序时，它总是有这样的代码。

```rust
fn main() {
    println!("Hello, world!");
}
```

- `fn`的意思是函数。
- `main`是启动程序的函数。

- `()`表示我们没有给函数任何变量来启动。

`{}`被称为**代码块**。这是代码所在的空间。

`println!`是一个**宏**，打印到控制台。一个**宏**就像一个函数，为你写代码。宏后面有一个`!`。我们以后会学习如何创建宏。现在，请记住，`!`表示它是一个宏。

为了学习`;`，我们将创建另一个函数。首先，在`main`中，我们将打印一个数字8。

```rust
fn main() {
    println!("Hello, world number {}!", 8);
}
```

`println!`中的`{}`的意思是 "把变量放在这里面"。这样就会打印出`Hello, world number 8!`。


我们可以像之前一样，放更多的东西进去。

```rust
fn main() {
    println!("Hello, worlds number {} and {}!", 8, 9);
}
```

这将打印出 `Hello, worlds number 8 and 9!`。

现在我们来创建函数。

```rust
fn number() -> i32 {
    8
}

fn main() {
    println!("Hello, world number {}!", number());
}
```

这也会打印出 `Hello, world number 8!`。当Rust查看`number()`时，它看到一个函数。这个函数:

- 没有参数(因为它有`()`)
- 返回一个`i32`。`->`(称为 "瘦箭")显示了函数返回的内容

函数内部只有`8`。因为没有`;`，所以这就是它返回的值。如果它有一个`;`，它将不会返回任何东西(它会返回一个`()`)。如果它有 `;`，Rust 不会编译通过，因为需要返回的是 `i32`，而 `;` 返回 `()`，不是 `i32`。

```rust
fn main() {
    println!("Hello, world number {}", number());
}

fn number() -> i32 {
    8;  // ⚠️
}
```

```text
5 | fn number() -> i32 {
  |    ------      ^^^ expected `i32`, found `()`
  |    |
  |    implicitly returns `()` as its body has no tail or `return` expression
6 |     8;
  |      - help: consider removing this semicolon
```

这意味着 "你告诉我`number()`返回的是`i32`，但你加了一个`;`，所以它什么都不返回"。所以编译器建议去掉分号。

你也可以写`return 8;`，但在Rust中，正常情况下只需将`;`改为`return`即可。

当你想给一个函数赋予变量时，把它们放在`()`里面。你必须给它们起个名字，写上类型。

```rust
fn multiply(number_one: i32, number_two: i32) { // Two i32s will enter the function. We will call them number_one and number_two.
    let result = number_one * number_two;
    println!("{} times {} is {}", number_one, number_two, result);
}

fn main() {
    multiply(8, 9); // We can give the numbers directly
    let some_number = 10; // Or we can declare two variables
    let some_other_number = 2;
    multiply(some_number, some_other_number); // and put them in the function
}
```

我们也可以返回一个`i32`。只要把最后的分号去掉就可以了:

```rust
fn multiply(number_one: i32, number_two: i32) -> i32 {
    let result = number_one * number_two;
    println!("{} times {} is {}", number_one, number_two, result);
    result // this is the i32 that we return
}

fn main() {
    let multiply_result = multiply(8, 9); // We used multiply() to print and to give the result to multiply_result
}
```

### 声明变量和代码块

使用`let`声明一个变量(声明一个变量=告诉Rust创建一个变量)。

```rust
fn main() {
    let my_number = 8;
    println!("Hello, number {}", my_number);
}
```

变量在代码块`{}`内开始和结束。在这个例子中，`my_number`在我们调用`println!`之前结束，因为它在自己的代码块里面。

```rust
fn main() {
    {
        let my_number = 8; // my_number starts here
                           // my_number ends here!
    }

    println!("Hello, number {}", my_number); // ⚠️ there is no my_number and
                                             // println!() can't find it
}
```

你可以使用代码块来返回一个值。

```rust
fn main() {
    let my_number = {
    let second_number = 8;
        second_number + 9 // No semicolon, so the code block returns 8 + 9.
                          // It works just like a function
    };

    println!("My number is: {}", my_number);
}
```

如果在代码块内部添加分号，它将返回 `()` (无)。

```rust
fn main() {
    let my_number = {
    let second_number = 8; // declare second_number,
        second_number + 9; // add 9 to second_number
                           // but we didn't return it!
                           // second_number dies now
    };

    println!("My number is: {:?}", my_number); // my_number is ()
}
```

那么为什么我们要写`{:?}`而不是`{}`呢？我们现在就来谈谈这个问题。

## 显示和调试

Rust中简单的变量可以用`{}`里面的`println!`打印。但是有些变量不能，你需要**debug print**。Debug打印是给程序员打印的，因为它通常会显示更多的信息。Debug有时看起来并不漂亮，因为它有额外的信息来帮助你。

你怎么知道你是否需要`{:?}`而不是`{}`？编译器会告诉你。比如说

```rust
fn main() {
    let doesnt_print = ();
    println!("This will not print: {}", doesnt_print); // ⚠️
}
```

当我们运行这个时，编译器会说:

```text
error[E0277]: `()` doesn't implement `std::fmt::Display`
 --> src\main.rs:3:41
  |
3 |     println!("This will not print: {}", doesnt_print);
  |                                         ^^^^^^^^^^^^ `()` cannot be formatted with the default formatter
  |
  = help: the trait `std::fmt::Display` is not implemented for `()`
  = note: in format strings you may be able to use `{:?}` (or {:#?} for pretty-print) instead
  = note: required by `std::fmt::Display::fmt`
  = note: this error originates in a macro (in Nightly builds, run with -Z macro-backtrace for more info)
```

信息比较多，但重要的部分是 `you may be able to use {:?} (or {:#?} for pretty-print) instead`. 这意味着你可以试试`{:?}`，也可以试试`{:#?}` `{:#?}`叫做 "漂亮打印"。它和`{:?}`一样，但是在更多的行上打印出不同的格式。

所以Display就是用`{}`打印，Debug就是用`{:?}`打印。

还有一点:如果你不想要新的一行，你也可以使用`print!`而不用`ln`。

```rust
fn main() {
    print!("This will not print a new line");
    println!(" so this will be on the same line");
}
```

这将打印`This will not print a new line so this will be on the same line`。

### 最小和最大的数

如果你想看最小和最大的数字，你可以用MIN和MAX。`std`的意思是 "标准库"，拥有Rust的所有主要函数等。我们将在以后学习标准库。但与此同时，你可以记住，这就是你如何获得一个类型的最小和最大的数字。

```rust
fn main() {
    println!("The smallest i8 is {} and the biggest i8 is {}.", std::i8::MIN, std::i8::MAX); // hint: printing std::i8::MIN means "print MIN inside of the i8 section in the standard library"
    println!("The smallest u8 is {} and the biggest u8 is {}.", std::u8::MIN, std::u8::MAX);
    println!("The smallest i16 is {} and the biggest i16 is {}.", std::i16::MIN, std::i16::MAX);
    println!("The smallest u16 is {} and the biggest u16 is {}.", std::u16::MIN, std::u16::MAX);
    println!("The smallest i32 is {} and the biggest i32 is {}.", std::i32::MIN, std::i32::MAX);
    println!("The smallest u32 is {} and the biggest u32 is {}.", std::u32::MIN, std::u32::MAX);
    println!("The smallest i64 is {} and the biggest i64 is {}.", std::i64::MIN, std::i64::MAX);
    println!("The smallest u64 is {} and the biggest u64 is {}.", std::u64::MIN, std::u64::MAX);
    println!("The smallest i128 is {} and the biggest i128 is {}.", std::i128::MIN, std::i128::MAX);
    println!("The smallest u128 is {} and the biggest u128 is {}.", std::u128::MIN, std::u128::MAX);

}
```

将会打印:

```text
The smallest i8 is -128 and the biggest i8 is 127.
The smallest u8 is 0 and the biggest u8 is 255.
The smallest i16 is -32768 and the biggest i16 is 32767.
The smallest u16 is 0 and the biggest u16 is 65535.
The smallest i32 is -2147483648 and the biggest i32 is 2147483647.
The smallest u32 is 0 and the biggest u32 is 4294967295.
The smallest i64 is -9223372036854775808 and the biggest i64 is 9223372036854775807.
The smallest u64 is 0 and the biggest u64 is 18446744073709551615.
The smallest i128 is -170141183460469231731687303715884105728 and the biggest i128 is 170141183460469231731687303715884105727.
The smallest u128 is 0 and the biggest u128 is 340282366920938463463374607431768211455.
```

## 可变性

当你用`let`声明一个变量时，它是不可改变的(不能改变)。

这将无法工作:

```rust
fn main() {
    let my_number = 8;
    my_number = 10; // ⚠️
}
```

编译器说:`error[E0384]: cannot assign twice to immutable variable my_number`。这是因为如果你只写`let`，变量是不可变的。

但有时你想改变你的变量。要创建一个可以改变的变量，就在`let`后面加上`mut`。

```rust
fn main() {
    let mut my_number = 8;
    my_number = 10;
}
```

现在没有问题了。

但是，你不能改变类型:甚至`mut`也不能让你这样做:这将无法工作。

```rust
fn main() {
    let mut my_variable = 8; // it is now an i32. That can't be changed
    my_variable = "Hello, world!"; // ⚠️
}
```

你会看到编译器发出的同样的 "预期"信息。`expected integer, found &str`. `&str`是一个字符串类型，我们很快就会知道。

### 遮蔽

shadowing是指使用`let`声明一个与另一个变量同名的新变量。它看起来像可变性，但完全不同。shadowing看起来是这样的:

```rust
fn main() {
    let my_number = 8; // This is an i32
    println!("{}", my_number); // prints 8
    let my_number = 9.2; // This is an f64 with the same name. But it's not the first my_number - it is completely different!
    println!("{}", my_number) // Prints 9.2
}
```

这里我们说我们用一个新的 "let绑定"对`my_number`进行了 "shadowing"。

那么第一个`my_number`是否被销毁了呢？没有，但是当我们调用`my_number`时，我们现在得到`my_number`的`f64`。因为它们在同一个作用域块中(同一个 `{}`)，我们不能再看到第一个 `my_number`。

但如果它们在不同的块中，我们可以同时看到两个。
 例如:

```rust
fn main() {
    let my_number = 8; // This is an i32
    println!("{}", my_number); // prints 8
    {
        let my_number = 9.2; // This is an f64. It is not my_number - it is completely different!
        println!("{}", my_number) // Prints 9.2
                                  // But the shadowed my_number only lives until here.
                                  // The first my_number is still alive!
    }
    println!("{}", my_number); // prints 8
}
```

因此，当你对一个变量进行shadowing处理时，你不会破坏它。你**屏蔽**了它。

那么shadowing的好处是什么呢？当你需要经常改变一个变量的时候，shadowing是很好的。想象一下，你想用一个变量做很多简单的数学运算。

```rust
fn times_two(number: i32) -> i32 {
    number * 2
}

fn main() {
    let final_number = {
        let y = 10;
        let x = 9; // x starts at 9
        let x = times_two(x); // shadow with new x: 18
        let x = x + y; // shadow with new x: 28
        x // return x: final_number is now the value of x
    };
    println!("The number is now: {}", final_number)
}
```

如果没有shadowing，你将不得不考虑不同的名称，尽管你并不关心x。

```rust
fn times_two(number: i32) -> i32 {
    number * 2
}

fn main() {
    // Pretending we are using Rust without shadowing
    let final_number = {
        let y = 10;
        let x = 9; // x starts at 9
        let x_twice = times_two(x); // second name for x
        let x_twice_and_y = x_twice + y; // third name for x!
        x_twice_and_y // too bad we didn't have shadowing - we could have just used x
    };
    println!("The number is now: {}", final_number)
}
```

一般来说，你在Rust中看到的shadowing就是这种情况。它发生在你想快速取用变量，对它做一些事情，然后再做其他事情的地方。而你通常将它用于那些你不太关心的快速变量。

## 栈、堆和指针

栈、堆和指针在Rust中非常重要。

栈和堆是计算机中保存内存的两个地方。重要的区别是:

栈的速度非常快, 但堆的速度就不那么快了. 它也不是超慢，但栈总是更快。但是你不能一直使用栈，因为:
- Rust需要在编译时知道一个变量的大小。所以像`i32`这样的简单变量就放在堆栈上，因为我们知道它们的确切大小。你总是知道`i32`要4字节，因为32位=4字节。所以`i32`总是可以放在栈上。
- 但有些类型在编译时不知道大小。但是栈需要知道确切的大小。那么你该怎么做呢？首先你把数据放在堆中，因为堆中可以有任何大小的数据。然后为了找到它，一个指针就会进入栈。这很好，因为我们总是知道指针的大小。所以，计算机就会先去栈，读取指针，然后跟着指针到数据所在的堆。

指针听起来很复杂，但它们很容易。指针就像一本书的目录。想象一下这本书。

```text
MY BOOK

TABLE OF CONTENTS

Chapter                        Page
Chapter 1: My life              1
Chapter 2: My cat               15
Chapter 3: My job               23
Chapter 4: My family            30
Chapter 5: Future plans         43
```

所以这就像五个指针。你可以阅读它们，找到它们所说的信息。"我的生活"这一章在哪里？在第1页(它*指向*第1页)。"我的工作"这一章在哪里？它在第23页。

在Rust中通常看到的指针叫做**引用**。这是重要的部分，要知道:一个引用指向另一个值的内存。引用意味着你*借*了这个值，但你并不拥有它。这和我们的书一样:目录并不拥有信息。章节才是信息的主人。在Rust中，引用文献的前面有一个`&`。所以:

- `let my_variable = 8`是一个普通的变量，但是:
- `let my_reference = &my_variable`是一个引用。

你把 `my_reference = &my_variable` 读成这样: "my_reference是对my_variable的引用". 或者:"my_reference是对my_variable的引用"。

这意味着`my_reference`只看`my_variable`的数据。`my_variable`仍然拥有它的数据。

你也可以有一个引用的引用，或者任何数量的引用。

```rust
fn main() {
    let my_number = 15; // This is an i32
    let single_reference = &my_number; //  This is a &i32
    let double_reference = &single_reference; // This is a &&i32
    let five_references = &&&&&my_number; // This is a &&&&&i32
}
```

这些都是不同的类型，就像 "朋友的朋友"和 "朋友"不同一样。

## 关于打印的更多信息

在Rust中，你几乎可以用任何你想要的方式打印东西。这里有一些关于打印的事情需要知道。

添加 `\n` 将会产生一个新行，而 `\t` 将会产生一个标签。

```rust
fn main() {
    // Note: this is print!, not println!
    print!("\t Start with a tab\nand move to a new line");
}
```

这样就可以打印了。

```text
         Start with a tab
and move to a new line
```

`""`里面可以写过很多行都没有问题，但是要注意间距。

```rust
fn main() {
    // Note: After the first line you have to start on the far left.
    // If you write directly under println!, it will add the spaces
    println!("Inside quotes
you can write over
many lines
and it will print just fine.");

    println!("If you forget to write
    on the left side, the spaces
    will be added when you print.");
}
```

这个打印出来的。

```text
Inside quotes
you can write over
many lines
and it will print just fine.
If you forget to write
    on the left side, the spaces
    will be added when you print.
```

如果你想打印`\n`这样的字符(称为 "转义字符")，你可以多加一个`\`。

```rust
fn main() {
    println!("Here are two escape characters: \\n and \\t");
}
```

这样就可以打印了。

```text
Here are two escape characters: \n and \t
```

有时你有太多的 `"` 和转义字符，并希望 Rust 忽略所有的字符。要做到这一点，您可以在开头添加 `r#`，在结尾添加 `#`。

```rust
fn main() {
    println!("He said, \"You can find the file at c:\\files\\my_documents\\file.txt.\" Then I found the file."); // We used \ five times here
    println!(r#"He said, "You can find the file at c:\files\my_documents\file.txt." Then I found the file."#)
}
```

这打印的是同样的东西，但使用 `r#` 使人类更容易阅读。

```text
He said, "You can find the file at c:\files\my_documents\file.txt." Then I found the file.
He said, "You can find the file at c:\files\my_documents\file.txt." Then I found the file.
```

如果你需要在里面打印`#`，那么你可以用`r##`开头，用`##`结尾。如果你需要打印多个连续的`#`，可以在每边多加一个#。

下面是四个例子。

```rust
fn main() {

    let my_string = "'Ice to see you,' he said."; // single quotes
    let quote_string = r#""Ice to see you," he said."#; // double quotes
    let hashtag_string = r##"The hashtag #IceToSeeYou had become very popular."##; // Has one # so we need at least ##
    let many_hashtags = r####""You don't have to type ### to use a hashtag. You can just use #.""####; // Has three ### so we need at least ####

    println!("{}\n{}\n{}\n{}\n", my_string, quote_string, hashtag_string, many_hashtags);

}
```

这将打印:

```text
'Ice to see you,' he said.
"Ice to see you," he said.
The hashtag #IceToSeeYou had become very popular.
"You don't have to type ### to use a hashtag. You can just use #."
```

`r#`还有另一个用途:使用它，你可以使用关键字(如`let`、`fn`等)作为变量名。

```rust
fn main() {
    let r#let = 6; // The variable's name is let
    let mut r#mut = 10; // This variable's name is mut
}
```

`r#`之所以有这个功能，是因为旧版本的Rust的关键字比现在的Rust少。所以有了`r#`就可以避免以前不是关键字的变量名的错误。

又或者因为某些原因，你*确实*需要一个函数的名字，比如`return`。那么你可以这样写:

```rust
fn r#return() -> u8 {
    println!("Here is your number.");
    8
}

fn main() {
    let my_number = r#return();
    println!("{}", my_number);
}
```

这样打印出来的结果是:

```text
Here is your number.
8
```

所以你可能不需要它，但是如果你真的需要为一个变量使用一个关键字，那么你可以使用`r#`。



如果你想打印`&str`或`char`的字节，你可以在字符串前写上`b`就可以了。这适用于所有ASCII字符。这些是所有的ASCII字符。

```text
☺☻♥♦♣♠♫☼►◄↕‼¶§▬↨↑↓→∟↔▲▼123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~
```

所以，当你打印这个

```rust
fn main() {
    println!("{:?}", b"This will look like numbers");
}
```

这就是结果:

```text
[84, 104, 105, 115, 32, 119, 105, 108, 108, 32, 108, 111, 111, 107, 32, 108, 105, 107, 101, 32, 110, 117, 109, 98, 101, 114, 115]
```

对于`char`来说，这叫做一个*字节*，对于`&str`来说，这叫做一个*字节字符串*。



如果你需要的话，也可以把`b`和`r`放在一起。

```rust
fn main() {
    println!("{:?}", br##"I like to write "#"."##);
}
```

这将打印出 `[73, 32, 108, 105, 107, 101, 32, 116, 111, 32, 119, 114, 105, 116, 101, 32, 34, 35, 34, 46]`。



还有一个Unicode转义，可以让你在字符串中打印任何Unicode字符: `\u{}`。`{}`里面有一个十六进制数字可以打印。下面是一个简短的例子，说明如何获得Unicode数字，以及如何再次打印它。

```rust
fn main() {
    println!("{:X}", '행' as u32); // Cast char as u32 to get the hexadecimal value
    println!("{:X}", 'H' as u32);
    println!("{:X}", '居' as u32);
    println!("{:X}", 'い' as u32);

    println!("\u{D589}, \u{48}, \u{5C45}, \u{3044}"); // Try printing them with unicode escape \u
}
```



我们知道，`println!`可以和`{}`(用于显示)或`{:?}`(用于调试)一起打印，再加上`{:#?}`就可以进行漂亮的打印。但是还有很多其他的打印方式。

例如，如果你有一个引用，你可以用`{:p}`来打印*指针地址*。指针地址指的是电脑内存中的位置。

```rust
fn main() {
    let number = 9;
    let number_ref = &number;
    println!("{:p}", number_ref);
}
```

这可以打印`0xe2bc0ffcfc`或其他地址。每次可能都不一样，这取决于你的计算机存储的位置。

或者你可以打印二进制、十六进制和八进制。

```rust
fn main() {
    let number = 555;
    println!("Binary: {:b}, hexadecimal: {:x}, octal: {:o}", number, number, number);
}
```

这将打印出`Binary: 1000101011, hexadecimal: 22b, octal: 1053`。

或者你可以添加数字来改变顺序。第一个变量将在索引0中，下一个在索引1中，以此类推。

```rust
fn main() {
    let father_name = "Vlad";
    let son_name = "Adrian Fahrenheit";
    let family_name = "Țepeș";
    println!("This is {1} {2}, son of {0} {2}.", father_name, son_name, family_name);
}
```

`father_name`在0位，`son_name`在1位，`family_name`在2位。所以它打印的是`This is Adrian Fahrenheit Țepeș, son of Vlad Țepeș`。


也许你有一个非常复杂的字符串要打印，`{}`大括号内有太多的变量。或者你需要不止一次的打印一个变量。那么在`{}`中添加名称就会有帮助。

```rust
fn main() {
    println!(
        "{city1} is in {country} and {city2} is also in {country},
but {city3} is not in {country}.",
        city1 = "Seoul",
        city2 = "Busan",
        city3 = "Tokyo",
        country = "Korea"
    );
}
```

这样就可以打印了。

```text
Seoul is in Korea and Busan is also in Korea,
but Tokyo is not in Korea.
```


如果你愿意，也可以在Rust中进行非常复杂的打印。下面展示怎样做：

{variable:padding alignment minimum.maximum}

要理解这一点，请看

1) 你想要一个变量名吗？先写出来，就像我们上面写{country}一样。
(如果你想做更多的事情，就在后面加一个`:`)
2) 你想要一个填充字符吗？例如，55加上三个 "填充零"就像00055。
3) padding的对齐方式(左/中/右)？
4) 你想要一个最小长度吗？(写一个数字就可以了) 
5) 你想要一个最大长度吗？(写一个数字，前面有一个`.`)

例如，我想写 "a"，左边有五个ㅎ，右边有五个ㅎ。

```rust
fn main() {
    let letter = "a";
    println!("{:ㅎ^11}", letter);
}
```

这样打印出来的结果是`ㅎㅎㅎㅎㅎaㅎㅎㅎㅎㅎ`。我们看看1)到5)的这个情况，就能明白编译器是怎么解读的：

- 你要不要变量名？`{:ㅎ^11}`没有变量名。`:`之前没有任何内容。
- 你需要一个填充字符吗？`{:ㅎ^11}` 是的:ㅎ"在`:`后面，有一个`^`。`<`表示变量在填充字符左边，`>`表示在填充字符右边，`^`表示在填充字符中间。
- 要不要设置最小长度？`{:ㅎ^11}`是:后面有一个11。
- 你想要一个最大长度吗？`{:ㅎ^11}` 不是:前面没有`.`的数字。

下面是多种类型的格式化的例子:


```rust
fn main() {
    let title = "TODAY'S NEWS";
    println!("{:-^30}", title); // no variable name, pad with -, put in centre, 30 characters long
    let bar = "|";
    println!("{: <15}{: >15}", bar, bar); // no variable name, pad with space, 15 characters each, one to the left, one to the right
    let a = "SEOUL";
    let b = "TOKYO";
    println!("{city1:-<15}{city2:->15}", city1 = a, city2 = b); // variable names city1 and city2, pad with -, one to the left, one to the right
}
```

它打印出来了。

```text
---------TODAY'S NEWS---------
|                            |
SEOUL--------------------TOKYO
```

## 字符串

Rust有两种主要类型的字符串。`String`和`&str`. 有什么区别呢？

- `&str`是一个简单的字符串。当你写`let my_variable = "Hello, world!"`时，你会创建一个`&str`。`&str`是非常快的。
- `String`是一个更复杂的字符串。它比较慢，但它有更多的功能。`String`是一个指针，数据在堆上。

另外注意，`&str`前面有`&`，因为你需要一个引用来使用`str`。这是因为我们上面看到的原因:堆需要知道大小。所以我们给它一个`&`，它知道大小，然后它就高兴了。另外，因为你用一个`&`与一个`str`交互，你并不拥有它。但是一个`String`是一个*拥有*的类型。我们很快就会知道为什么这一点很重要。

`&str`和`String`都是UTF-8。例如，你可以写

```rust
fn main() {
    let name = "서태지"; // This is a Korean name. No problem, because a &str is UTF-8.
    let other_name = String::from("Adrian Fahrenheit Țepeș"); // Ț and ș are no problem in UTF-8.
}
```

你可以在`String::from("Adrian Fahrenheit Țepeș")`中看到，很容易从`&str`中创建一个`String`。这两种类型虽然不同，但联系非常紧密。

你甚至可以写表情符号，这要感谢UTF-8。

```rust
fn main() {
    let name = "😂";
    println!("My name is actually {}", name);
}
```

在你的电脑上，会打印`My name is actually 😂`，除非你的命令行不能打印。那么它会显示`My name is actually �`。但Rust对emojis或其他Unicode没有问题。

我们再来看看`str`使用`&`的原因，以确保我们理解。

- `str`是一个动态大小的类型(动态大小=大小可以不同)。比如 "서태지"和 "Adrian Fahrenheit Țepeș"这两个名字的大小是不一样的。

```rust
fn main() {

    println!("A String is always {:?} bytes. It is Sized.", std::mem::size_of::<String>()); // std::mem::size_of::<Type>() gives you the size in bytes of a type
    println!("And an i8 is always {:?} bytes. It is Sized.", std::mem::size_of::<i8>());
    println!("And an f64 is always {:?} bytes. It is Sized.", std::mem::size_of::<f64>());
    println!("But a &str? It can be anything. '서태지' is {:?} bytes. It is not Sized.", std::mem::size_of_val("서태지")); // std::mem::size_of_val() gives you the size in bytes of a variable
    println!("And 'Adrian Fahrenheit Țepeș' is {:?} bytes. It is not Sized.", std::mem::size_of_val("Adrian Fahrenheit Țepeș"));
}
```

这个打印:

```text
A String is always 24 bytes. It is Sized.
And an i8 is always 1 bytes. It is Sized.
And an f64 is always 8 bytes. It is Sized.
But a &str? It can be anything. '서태지' is 9 bytes. It is not Sized.
And 'Adrian Fahrenheit Țepeș' is 25 bytes. It is not Sized.
```

这就是为什么我们需要一个 &，因为 `&` 是一个指针，而 Rust 知道指针的大小。所以指针会放在栈中。如果我们写`str`，Rust就不知道该怎么做了，因为它不知道指针的大小。



有很多方法可以创建`String`。下面是一些。

- `String::from("This is the string text");` 这是String的一个方法，它接受文本并创建一个String.
- `"This is the string text".to_string()`. 这是&str的一个方法，使其成为一个String。
- `format!` 宏。
 这和`println!`一样，只是它创建了一个字符串，而不是打印。所以你可以这样做:

```rust
fn main() {
    let my_name = "Billybrobby";
    let my_country = "USA";
    let my_home = "Korea";

    let together = format!(
        "I am {} and I come from {} but I live in {}.",
        my_name, my_country, my_home
    );
}
```

现在我们有了一个一起命名的字符串，但还没有打印出来。

还有一种创建String的方法叫做`.into()`，但它有点不同，因为`.into()`并不只是用来创建`String`。有些类型可以很容易地使用`From`和`.into()`转换为另一种类型，并从另一种类型转换出来。而如果你有`From`，那么你也有`.into()`。`From` 更加清晰，因为你已经知道了类型:你知道 `String::from("Some str")` 是一个来自 `&str` 的 `String`。但是对于`.into()`，有时候编译器并不知道。

```rust
fn main() {
    let my_string = "Try to make this a String".into(); // ⚠️
}
```

Rust不知道你要的是什么类型，因为很多类型都可以从一个`&str`创建出来。它说:"我可以把一个&str做成很多东西。你想要哪一种？"

```text
error[E0282]: type annotations needed
 --> src\main.rs:2:9
  |
2 |     let my_string = "Try to make this a String".into();
  |         ^^^^^^^^^ consider giving `my_string` a type
```

所以你可以这样做:

```rust
fn main() {
    let my_string: String = "Try to make this a String".into();
}
```

现在你得到了一个字符串。

## const和static

有两种声明值的方法，不仅仅是用`let`。它们是`const`和`static`。另外，Rust不会使用类型推理：你需要为它们编写类型。这些都是用于不改变的值（`const`意味着常量）。区别在于:

- `const`是用于不改变的值，当使用它时，名字会被替换成值。
- `static`与`const`类似，但有一个固定的内存位置，可以作为一个全局变量使用。

所以它们几乎是一样的。Rust程序员几乎总是使用`const`。

一般用全大写字母作为名字，而且通常在`main`之外，这样它们就可以在整个程序中生存。

两个例子是 `const NUMBER_OF_MONTHS: u32 = 12;` 和 `static SEASONS: [&str; 4] = ["Spring", "Summer", "Fall", "Winter"];`

## 关于引用的更多信息

引用在Rust中非常重要。Rust使用引用来确保所有的内存访问是安全的。我们知道，我们使用`&`来创建一个引用。

```rust
fn main() {
    let country = String::from("Austria");
    let ref_one = &country;
    let ref_two = &country;

    println!("{}", ref_one);
}
```

这样就会打印出`Austria`。

在代码中，`country`是一个`String`。然后我们创建了两个`country`的引用。它们的类型是`&String`，你说这是一个 "字符串的引用"。我们可以创建三个引用或者一百个对 `country` 的引用，这都没有问题。

但这是一个问题。

```rust
fn return_str() -> &str {
    let country = String::from("Austria");
    let country_ref = &country;
    country_ref // ⚠️
}

fn main() {
    let country = return_str();
}
```

`return_str()`函数创建了一个String，然后它创建了一个对String的引用。然后它试图返回引用。但是`country`这个String只活在函数里面，然后它就死了。一旦一个变量消失了，计算机就会清理内存，并将其用于其他用途。所以在函数结束后，`country_ref`引用的是已经消失的内存，这是不对的。Rust防止我们在这里犯内存的错误。

这就是我们上面讲到的 "拥有"类型的重要部分。因为你拥有一个`String`，你可以把它传给别人。但是如果 `&String` 的 `String` 死了，那么 `&String` 就会死掉，所以你不能把它的 "所有权"传给别人。

## 可变引用

如果您想使用一个引用来改变数据，您可以使用一个可变引用。对于可变引用，您可以写 `&mut` 而不是 `&`。

```rust
fn main() {
    let mut my_number = 8; // don't forget to write mut here!
    let num_ref = &mut my_number;
}
```

那么这两种类型是什么呢？`my_number`是`i32`，`num_ref`是`&mut i32`(我们说是 "可变引用`i32`")。

所以我们用它来给my_number加10。但是你不能写`num_ref += 10`，因为`num_ref`不是`i32`的值，它是一个`&i32`。其实这个值就在`i32`里面。为了达到值所在的地方，我们用`*`。`*`的意思是 "我不要引用，我要引用对应的值"。换句话说，一个`*`与`&`是相反的。另外，一个`*`抹去了一个`&`。

```rust
fn main() {
    let mut my_number = 8;
    let num_ref = &mut my_number;
    *num_ref += 10; // Use * to change the i32 value.
    println!("{}", my_number);

    let second_number = 800;
    let triple_reference = &&&second_number;
    println!("Second_number = triple_reference? {}", second_number == ***triple_reference);
}
```

这个打印:

```text
18
Second_number = triple_reference? true
```

因为使用`&`叫做 "引用"，所以使用`*`叫做 "**de**referencing"。

Rust有两个规则，分别是可变引用和不可变引用。它们非常重要，但也很容易记住，因为它们很有意义。

- **规则1**。如果你只有不可变引用，你可以有任意多的引用。1个也行，3个也行，1000个也行，没问题。
- **规则2**: 如果你有一个可变引用，你只能有一个。另外，你不能同时使用一个不可变引用**和**一个可变引用。

这是因为可变引用可以改变数据。如果你在其他引用读取数据时改变数据，你可能会遇到问题。


一个很好的理解方式是思考一个Powerpoint演示。

情况一是关于**只有一个可变引用**

情境一 一个员工正在编写一个Powerpoint演示文稿，他希望他的经理能帮助他。该员工将自己的登录信息提供给经理，并请他帮忙进行编辑。现在，经理对该员工的演示文稿有了一个 "可变引用"。经理可以做任何他想做的修改，然后把电脑还给他。这很好，因为没有人在看这个演示文稿。

情况二是关于**只有不可变引用**

情况二 该员工要给100个人做演示。现在这100个人都可以看到该员工的数据。
 他们都有一个 "不可改变的引用"，即员工的介绍。这很好，因为他们可以看到它，但没有人可以改变数据。

情况三是**有问题的情况**

情况三 员工把他的登录信息给了经理 他的经理现在有了一个 "可变引用"。然后员工去给100个人做演示，但是经理还是可以登录。这是不对的，因为经理可以登录，可以做任何事情。也许他的经理会登录电脑，然后开始给他的母亲打一封邮件! 现在这100人不得不看着经理给他母亲写邮件，而不是演示。这不是他们期望看到的。

下面是一个可变借用与不可变借用的例子:

```rust
fn main() {
    let mut number = 10;
    let number_ref = &number;
    let number_change = &mut number;
    *number_change += 10;
    println!("{}", number_ref); // ⚠️
}
```

编译器打印了一个有用的信息来告诉我们问题所在。

```text
error[E0502]: cannot borrow `number` as mutable because it is also borrowed as immutable
 --> src\main.rs:4:25
  |
3 |     let number_ref = &number;
  |                      ------- immutable borrow occurs here
4 |     let number_change = &mut number;
  |                         ^^^^^^^^^^^ mutable borrow occurs here
5 |     *number_change += 10;
6 |     println!("{}", number_ref);
  |                    ---------- immutable borrow later used here
```

然而，这段代码可以工作。为什么会这样？

```rust
fn main() {
    let mut number = 10;
    let number_change = &mut number; // create a mutable reference
    *number_change += 10; // use mutable reference to add 10
    let number_ref = &number; // create an immutable reference
    println!("{}", number_ref); // print the immutable reference
}
```

它打印出`20`没有问题。它能工作是因为编译器足够聪明，能够理解我们的代码。它知道我们使用了`number_change`来改变`number`，但没有再使用它。所以这里没有问题。我们并没有将不可变和可变引用一起使用。

早期在Rust中，这种代码实际上会产生错误，但现在的编译器更聪明了。它不仅能理解我们输入的内容，还能理解我们如何使用所有的东西。

### 再谈shadowing

还记得我们说过，shadowing不会**破坏**一个值，而是**屏蔽**它吗？现在我们可以用引用来看看这个问题。

```rust
fn main() {
    let country = String::from("Austria");
    let country_ref = &country;
    let country = 8;
    println!("{}, {}", country_ref, country);
}
```

这是打印`Austria, 8`还是`8, 8`？它打印的是`Austria, 8`。首先我们声明一个`String`，叫做`country`。然后我们给这个字符串创建一个引用`country_ref`。然后我们用8来shadowing国家，这是一个`i32`。但是第一个`country`并没有被销毁，所以`country_ref`仍然写着 "Austria"，而不是 "8"。下面是同样的代码，并加了一些注释来说明它的工作原理。

```rust
fn main() {
    let country = String::from("Austria"); // Now we have a String called country
    let country_ref = &country; // country_ref is a reference to this data. It's not going to change
    let country = 8; // Now we have a variable called country that is an i8. But it has no relation to the other one, or to country_ref
    println!("{}, {}", country_ref, country); // country_ref still refers to the data of String::from("Austria") that we gave it.
}
```

## 函数的引用

引用对函数非常有用。Rust中关于值的规则是:一个值只能有一个所有者。

这段代码将无法工作:

```rust
fn print_country(country_name: String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Austria");
    print_country(country); // We print "Austria"
    print_country(country); // ⚠️ That was fun, let's do it again!
}
```

它不能工作，因为`country`被破坏了。下面是如何操作的。

- 第一步，我们创建`String`，称为`country`。`country`是所有者。
- 第二步:我们把`country`给`print_country`。`print_country`没有`->`，所以它不返回任何东西。`print_country`完成后，我们的`String`现在已经死了。
- 第三步:我们尝试把`country`给`print_country`，但我们已经这样做了。我们已经没有`country`可以给了。

我们可以让`print_country`给`String`回来，但是有点尴尬。

```rust
fn print_country(country_name: String) -> String {
    println!("{}", country_name);
    country_name // return it here
}

fn main() {
    let country = String::from("Austria");
    let country = print_country(country); // we have to use let here now to get the String back
    print_country(country);
}
```

现在打印出来了。

```text
Austria
Austria
```

更好的解决方法是增加`&`。

```rust
fn print_country(country_name: &String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Austria");
    print_country(&country); // We print "Austria"
    print_country(&country); // That was fun, let's do it again!
}
```

现在 `print_country()` 是一个函数，它接受 `String` 的引用: `&String`。另外，我们给country一个引用，写作`&country`。这表示 "你可以看它，但我要保留它"。

现在让我们用一个可变引用来做类似的事情。下面是一个使用可变变量的函数的例子:

```rust
fn add_hungary(country_name: &mut String) { // first we say that the function takes a mutable reference
    country_name.push_str("-Hungary"); // push_str() adds a &str to a String
    println!("Now it says: {}", country_name);
}

fn main() {
    let mut country = String::from("Austria");
    add_hungary(&mut country); // we also need to give it a mutable reference.
}
```

此打印`Now it says: Austria-Hungary`。

所以得出结论:

- `fn function_name(variable: String)`接收了`String`，并拥有它。如果它不返回任何东西，那么这个变量就会在函数里面死亡。
- `fn function_name(variable: &String)` 借用 `String` 并可以查看它
- `fn function_name(variable: &mut String)`借用`String`，可以更改。

下面是一个看起来像可变引用的例子，但它是不同的。

```rust
fn main() {
    let country = String::from("Austria"); // country is not mutable, but we are going to print Austria-Hungary. How?
    adds_hungary(country);
}

fn adds_hungary(mut country: String) { // Here's how: adds_hungary takes the String and declares it mutable!
    country.push_str("-Hungary");
    println!("{}", country);
}
```

这怎么可能呢？因为`mut country`不是引用。`adds_hungary`现在拥有`country`。(记住，它占用的是`String`而不是`&String`)。当你调用`adds_hungary`的那一刻，它就完全成了country的主人。`country`与`String::from("Austria")`没有关系了。所以，`adds_hungary`可以把`country`当作可变的，这样做是完全安全的。

还记得我们上面的员工Powerpoint和经理的情况吗？在这种情况下，就好比员工只是把自己的整台电脑交给了经理。员工不会再碰它，所以经理可以对它做任何他想做的事情。

## 拷贝类型

Rust中的一些类型非常简单。它们被称为**拷贝类型**。这些简单的类型都在栈中，编译器知道它们的大小。这意味着它们非常容易复制，所以当你把它发送到一个函数时，编译器总是会复制。它总是复制，因为它们是如此的小而简单，没有理由不复制。所以你不需要担心这些类型的所有权问题。

这些简单的类型包括:整数、浮点数、布尔值(`true`和`false`)和`char`。

如何知道一个类型是否**实现**复制？(实现 = 能够使用)你可以查看文档。例如，这里是 char 的文档:

[https://doc.rust-lang.org/std/primitive.char.html](https://doc.rust-lang.org/std/primitive.char.html)

在左边你可以看到**Trait Implementations**。例如你可以看到**Copy**, **Debug**, 和 **Display**。所以你知道，当你把一个`char`:

- 当你把它发送到一个函数(**Copy**)时，它就被复制了。
- 可以用`{}`打印(**Display**)
- 可以用`{:?}`打印(**Debug**)

```rust
fn prints_number(number: i32) { // There is no -> so it's not returning anything
                             // If number was not copy type, it would take it
                             // and we couldn't use it again
    println!("{}", number);
}

fn main() {
    let my_number = 8;
    prints_number(my_number); // Prints 8. prints_number gets a copy of my_number
    prints_number(my_number); // Prints 8 again.
                              // No problem, because my_number is copy type!
}
```

但是如果你看一下String的文档，它不是拷贝类型。

[https://doc.rust-lang.org/std/string/struct.String.html](https://doc.rust-lang.org/std/string/struct.String.html)

在左边的**Trait Implementations**中，你可以按字母顺序查找。A、B、C......C中没有**Copy**，但是有**Clone**。**Clone**和**Copy**类似，但通常需要更多的内存。另外，你必须用`.clone()`来调用它--它不会自己克隆。

在这个例子中，`prints_country()`打印的是国家名称，一个`String`。我们想打印两次，但我们不能。

```rust
fn prints_country(country_name: String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Kiribati");
    prints_country(country);
    prints_country(country); // ⚠️
}
```

但现在我们明白了这个信息。

```text
error[E0382]: use of moved value: `country`
 --> src\main.rs:4:20
  |
2 |     let country = String::from("Kiribati");
  |         ------- move occurs because `country` has type `std::string::String`, which does not implement the `Copy` trait
3 |     prints_country(country);
  |                    ------- value moved here
4 |     prints_country(country);
  |                    ^^^^^^^ value used here after move
```

重要的部分是`which does not implement the Copy trait`。但是在文档中我们看到String实现了`Clone`的特性。所以我们可以在代码中添加`.clone()`。这样就创建了一个克隆，然后我们将克隆发送到函数中。现在 `country` 还活着，所以我们可以使用它。

```rust
fn prints_country(country_name: String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Kiribati");
    prints_country(country.clone()); // make a clone and give it to the function. Only the clone goes in, and country is still alive
    prints_country(country);
}
```

当然，如果`String`非常大，`.clone()`就会占用很多内存。一个`String`可以是一整本书的长度，我们每次调用`.clone()`都会复制这本书。所以，如果可以的话，使用`&`来做引用是比较快的。例如，这段代码将`&str`推送到`String`上，然后每次在函数中使用时都会进行克隆。

```rust
fn get_length(input: String) { // Takes ownership of a String
    println!("It's {} words long.", input.split_whitespace().count()); // splits to count the number of words
}

fn main() {
    let mut my_string = String::new();
    for _ in 0..50 {
        my_string.push_str("Here are some more words "); // push the words on
        get_length(my_string.clone()); // gives it a clone every time
    }
}
```

它的打印。

```text
It's 5 words long.
It's 10 words long.
...
It's 250 words long.
```

这就是50个克隆。这里是用引用代替更好:

```rust
fn get_length(input: &String) {
    println!("It's {} words long.", input.split_whitespace().count());
}

fn main() {
    let mut my_string = String::new();
    for _ in 0..50 {
        my_string.push_str("Here are some more words ");
        get_length(&my_string);
    }
}
```

不是50个克隆，而是0个。



### 无值变量

一个没有值的变量叫做 "未初始化"变量。未初始化的意思是 "还没有开始"。它们很简单:只需写上`let`和变量名。

```rust
fn main() {
    let my_variable; // ⚠️
}
```

但是你还不能使用它，如果任何东西都没有被初始化，Rust就不会编译。

但有时它们会很有用。一个很好的例子是当:

- 你有一个代码块，而你的变量值就在里面，并且
- 变量需要活在代码块之外。

```rust
fn loop_then_return(mut counter: i32) -> i32 {
    loop {
        counter += 1;
        if counter % 50 == 0 {
            break;
        }
    }
    counter
}

fn main() {
    let my_number;

    {
        // Pretend we need to have this code block
        let number = {
            // Pretend there is code here to make a number
            // Lots of code, and finally:
            57
        };

        my_number = loop_then_return(number);
    }

    println!("{}", my_number);
}
```

这将打印出 `100`。

你可以看到 `my_number` 是在 `main()` 函数中声明的，所以它一直活到最后。但是它的值是在循环里面得到的。然而，这个值和`my_number`一样长，因为`my_number`有这个值。而如果你在块里面写了`let my_number = loop_then_return(number)`，它就会马上死掉。

如果你简化代码，对想象是有帮助的。`loop_then_return(number)`给出的结果是100，所以我们删除它，改写`100`。另外，现在我们不需要 `number`，所以我们也删除它。现在它看起来像这样:

```rust
fn main() {
    let my_number;
    {
        my_number = 100;
    }

    println!("{}", my_number);
}
```

所以说`let my_number = { 100 };`差不多。

另外注意，`my_number`不是`mut`。我们在给它50之前并没有给它一个值，所以它的值一直没有改变。最后，`my_number`的真正代码只是`let my_number = 100;`。

## 集合类型

Rust有很多类型用于创建集合。当你需要在一个地方有多个值时，就可以使用集合。例如，你可以在一个变量中包含你所在国家的所有城市的信息。我们先从数组开始，数组的速度最快，但功能也最少。它们在这方面有点像`&str`。

### 数组

数组是方括号内的数据。`[]`. 数组:

- 不能改变其大小。
- 必须只包含相同的类型。

但是，它们的速度非常快。

数组的类型是:`[type; number]`。例如，`["One", "Two"]`的类型是`[&str; 2]`。这意味着，即使这两个数组也有不同的类型。

```rust
fn main() {
    let array1 = ["One", "Two"]; // This one is type [&str; 2]
    let array2 = ["One", "Two", "Five"]; // But this one is type [&str; 3]. Different type!
}
```

这里有一个很好的提示:要想知道一个变量的类型，你可以通过给编译器下坏指令来 "询问"它。比如说

```rust
fn main() {
    let seasons = ["Spring", "Summer", "Autumn", "Winter"];
    let seasons2 = ["Spring", "Summer", "Fall", "Autumn", "Winter"];
    seasons.ddd(); // ⚠️
    seasons2.thd(); // ⚠️ as well
}
```

编译器说:"什么？seasons没有`.ddd()`的方法，seasons2也没有`.thd()`的方法！！"你可以看到:

```text
error[E0599]: no method named `ddd` found for array `[&str; 4]` in the current scope
 --> src\main.rs:4:13
  |
4 |     seasons.ddd(); // 
  |             ^^^ method not found in `[&str; 4]`

error[E0599]: no method named `thd` found for array `[&str; 5]` in the current scope
 --> src\main.rs:5:14
  |
5 |     seasons2.thd(); // 
  |              ^^^ method not found in `[&str; 5]`
```

所以它告诉你`` method not found in `[&str; 4]` ``，这就是类型。

如果你想要一个数值都一样的数组，你可以这样声明。

```rust
fn main() {
    let my_array = ["a"; 10];
    println!("{:?}", my_array);
}
```

这样就打印出了`["a", "a", "a", "a", "a", "a", "a", "a", "a", "a"]`。

这个方法经常用来创建缓冲区。例如，`let mut buffer = [0; 640]`创建一个640个零的数组。然后我们可以将零改为其他数字，以便添加数据。

你可以用[]来索引(获取)数组中的条目。第一个条目是[0]，第二个是[1]，以此类推。

```rust
fn main() {
    let my_numbers = [0, 10, -20];
    println!("{}", my_numbers[1]); // prints 10
}
```

你可以得到一个数组的一个片断(一块)。首先你需要一个&，因为编译器不知道大小。然后你可以使用`..`来显示范围。

例如，让我们使用这个数组。`[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`.

```rust
fn main() {
    let array_of_ten = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    let three_to_five = &array_of_ten[2..5];
    let start_at_two = &array_of_ten[1..];
    let end_at_five = &array_of_ten[..5];
    let everything = &array_of_ten[..];

    println!("Three to five: {:?}, start at two: {:?}, end at five: {:?}, everything: {:?}", three_to_five, start_at_two, end_at_five, everything);
}
```

记住这一点。

- 索引号从0开始(不是1)
- 索引范围是**不包含的**(不包括最后一个数字)。

所以`[0..2]`是指第一个指数和第二个指数(0和1)。或者你也可以称它为 "零点和第一"指数。它没有第三项，也就是索引2。

你也可以有一个**包含的**范围，这意味着它也包括最后一个数字。要做到这一点。
 添加`=`，写成`..=`，而不是`..`。所以，如果你想要第一项、第二项和第三项，可以写成`[0..=2]`，而不是`[0..2]`。

## 向量

就像我们有`&str`和`String`一样，我们有数组和向量。数组的功能少了就快，向量的功能多了就慢。(当然，Rust的速度一直都是非常快的，所以向量并不慢，只是比数组慢*一点*)。类型写成`Vec`，你也可以直接叫它 "vec"。

向量的声明主要有两种方式。一种是像`String`一样使用`new`:

```rust
fn main() {
    let name1 = String::from("Windy");
    let name2 = String::from("Gomesy");

    let mut my_vec = Vec::new();
    // If we run the program now, the compiler will give an error.
    // It doesn't know the type of vec.

    my_vec.push(name1); // Now it knows: it's Vec<String>
    my_vec.push(name2);
}
```

你可以看到`Vec`里面总是有其他东西，这就是`<>`(角括号)的作用。`Vec<String>`是一个有一个或多个`String`的向量。你还可以在里面有更多的类型。比如说

- `Vec<(i32, i32)>` 这是一个 `Vec` 其中每个元素是一个元组。`(i32, i32)`.
- `Vec<Vec<String>>`这是一个`Vec`，其中有`Vec`的`Strings`。比如说你想把你喜欢的书保存为`Vec<String>`。然后你再用另一本书来做，就会得到另一个`Vec<String>`。为了保存这两本书，你会把它们放入另一个`Vec`中，这就是`Vec<Vec<String>>`。

与其使用 `.push()` 让 Rust 决定类型，不如直接声明类型。

```rust
fn main() {
    let mut my_vec: Vec<String> = Vec::new(); // The compiler knows the type
                                              // so there is no error.
}
```

你可以看到，向量中的元素必须具有相同的类型。

另一个创建向量的简单方法是使用 `vec!` 宏。它看起来像一个数组声明，但前面有 `vec!`。

```rust
fn main() {
    let mut my_vec = vec![8, 10, 10];
}
```

类型是`Vec<i32>`。你称它为 "i32的Vec"。而`Vec<String>`是 "String的Vec"。`Vec<Vec<String>>`是 "String的Vec的Vec"。

你也可以对一个向量进行分片，就像在数组中一样。

```rust
fn main() {
    let vec_of_ten = vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    // Everything is the same as above except we added vec!.
    let three_to_five = &vec_of_ten[2..5];
    let start_at_two = &vec_of_ten[1..];
    let end_at_five = &vec_of_ten[..5];
    let everything = &vec_of_ten[..];

    println!("Three to five: {:?},
start at two: {:?}
end at five: {:?}
everything: {:?}", three_to_five, start_at_two, end_at_five, everything);
}
```

因为Vector比数组慢，我们可以用一些方法让它更快。一个vec有一个**容量**，也就是给向量的空间。当你在向量上推送一个新的元素时，它会越来越接近容量。然后，如果你超过了容量，它将使其容量翻倍，并将元素复制到新的空间。这就是所谓的重新分配。我们将使用一种名为`.capacity()`的方法来查看向量的容量，在我们向它添加元素时。

例如，我们将使用名为`.capacity()`的方法来观察一个向量的容量。

```rust
fn main() {
    let mut num_vec = Vec::new();
    println!("{}", num_vec.capacity()); // 0 elements: prints 0
    num_vec.push('a'); // add one character
    println!("{}", num_vec.capacity()); // 1 element: prints 4. Vecs with 1 item always start with capacity 4
    num_vec.push('a'); // add one more
    num_vec.push('a'); // add one more
    num_vec.push('a'); // add one more
    println!("{}", num_vec.capacity()); // 4 elements: still prints 4.
    num_vec.push('a'); // add one more
    println!("{}", num_vec.capacity()); // prints 8. We have 5 elements, but it doubled 4 to 8 to make space
}
```

这个打印:

```text
0
4
4
8
```

所以这个向量有两次重分配: 0到4，4到8。我们可以让它更快:

```rust
fn main() {
    let mut num_vec = Vec::with_capacity(8); // Give it capacity 8
    num_vec.push('a'); // add one character
    println!("{}", num_vec.capacity()); // prints 8
    num_vec.push('a'); // add one more
    println!("{}", num_vec.capacity()); // prints 8
    num_vec.push('a'); // add one more
    println!("{}", num_vec.capacity()); // prints 8.
    num_vec.push('a'); // add one more
    num_vec.push('a'); // add one more // Now we have 5 elements
    println!("{}", num_vec.capacity()); // Still 8
}
```

这个向量有0个重分配，这是比较好的。所以如果你认为你知道你需要多少元素，你可以使用`Vec::with_capacity()`来使它更快。

你记得你可以用`.into()`把`&str`变成`String`。你也可以用它把一个数组变成`Vec`。你必须告诉 `.into()` 你想要一个 `Vec`，但你不必选择 `Vec` 的类型。如果你不想选择，你可以写`Vec<_>`。

```rust
fn main() {
    let my_vec: Vec<u8> = [1, 2, 3].into();
    let my_vec2: Vec<_> = [9, 0, 10].into(); // Vec<_> means "choose the Vec type for me"
                                             // Rust will choose Vec<i32>
}
```

## 元组

Rust中的元组使用`()`。我们已经见过很多空元组了，因为函数中的*nothing*实际上意味着一个空元组。

```text
fn do_something() {}
```

其实是它的简写:

```text
fn do_something() -> () {}
```

这个函数什么也得不到(一个空元组)，也不返回什么(一个空元组)。所以我们已经经常使用元组了。当你在一个函数中不返回任何东西时，你实际上返回的是一个空元组。

```rust
fn just_prints() {
    println!("I am printing"); // Adding ; means we return an empty tuple
}

fn main() {}
```

但是元组可以容纳很多东西，也可以容纳不同的类型。元组里面的元素也是用数字0、1、2等来做索引的，但要访问它们，你要用`.`而不是`[]`。让我们把一大堆类型放到一个元组中。

```rust
fn main() {
    let random_tuple = ("Here is a name", 8, vec!['a'], 'b', [8, 9, 10], 7.7);
    println!(
        "Inside the tuple is: First item: {:?}
Second item: {:?}
Third item: {:?}
Fourth item: {:?}
Fifth item: {:?}
Sixth item: {:?}",
        random_tuple.0,
        random_tuple.1,
        random_tuple.2,
        random_tuple.3,
        random_tuple.4,
        random_tuple.5,
    )
}
```

这个打印:

```text
Inside the tuple is: First item: "Here is a name"
Second item: 8
Third item: ['a']
Fourth item: 'b'
Fifth item: [8, 9, 10]
Sixth item: 7.7
```

这个元组的类型是 `(&str, i32, Vec<char>, char, [i32; 3], f64)`。


你可以使用一个元组来创建多个变量。看看这段代码。

```rust
fn main() {
    let str_vec = vec!["one", "two", "three"];
}
```

`str_vec`里面有三个元素。如果我们想把它们拉出来呢？这时我们可以使用元组。

```rust
fn main() {
    let str_vec = vec!["one", "two", "three"];

    let (a, b, c) = (str_vec[0], str_vec[1], str_vec[2]); // call them a, b, and c
    println!("{:?}", b);
}
```

这就打印出`"two"`，也就是`b`。这就是所谓的*解构*。这是因为首先变量是在结构体里面的，但是我们又做了`a`、`b`、`c`这些不是在结构体里面的变量。

如果你需要解构，但又不想要所有的变量，你可以使用`_`。

```rust
fn main() {
    let str_vec = vec!["one", "two", "three"];

    let (_, _, variable) = (str_vec[0], str_vec[1], str_vec[2]);
}
```

现在它只创建了一个叫`variable`的变量，但没有为其他值做变量。

还有很多集合类型，还有很多使用数组、vec和tuple的方法。我们也将学习更多关于它们的知识，但首先我们将学习控制流。

## 控制流

控制流的意思是告诉你的代码在不同的情况下该怎么做。最简单的控制流是`if`。

```rust
fn main() {
    let my_number = 5;
    if my_number == 7 {
        println!("It's seven");
    }
}
```

另外注意，你用的是`==`而不是`=`。`==`是用来比较的，`=`是用来*赋值*的(给一个值)。另外注意，我们写的是`if my_number == 7`而不是`if (my_number == 7)`。在Rust中，你不需要用`if`的括号。

`else if`和`else`给你更多的控制:

```rust
fn main() {
    let my_number = 5;
    if my_number == 7 {
        println!("It's seven");
    } else if my_number == 6 {
        println!("It's six")
    } else {
        println!("It's a different number")
    }
}
```

这打印出`It's a different number`，因为它不等于7或6。


您可以使用 `&&`(和)和 `||`(或)添加更多条件。

```rust
fn main() {
    let my_number = 5;
    if my_number % 2 == 1 && my_number > 0 { // % 2 means the number that remains after diving by two
        println!("It's a positive odd number");
    } else if my_number == 6 {
        println!("It's six")
    } else {
        println!("It's a different number")
    }
}
```

这打印出的是`It's a positive odd number`，因为当你把它除以2时，你有一个1的余数，它大于0。


你可以看到，过多的`if`、`else`和`else if`会很难读。在这种情况下，你可以使用`match`来代替，它看起来更干净。但是您必须为每一个可能的结果进行匹配。例如，这将无法工作:

```rust
fn main() {
    let my_number: u8 = 5;
    match my_number {
        0 => println!("it's zero"),
        1 => println!("it's one"),
        2 => println!("it's two"),
        // ⚠️
    }
}
```

编译器说:

```text
error[E0004]: non-exhaustive patterns: `3u8..=std::u8::MAX` not covered
 --> src\main.rs:3:11
  |
3 |     match my_number {
  |           ^^^^^^^^^ pattern `3u8..=std::u8::MAX` not covered
```

这就意味着 "你告诉我0到2，但`u8`可以到255。那3呢？那4呢？5呢？" 以此类推。所以你可以加上`_`，意思是 "其他任何东西"。

```rust
fn main() {
    let my_number: u8 = 5;
    match my_number {
        0 => println!("it's zero"),
        1 => println!("it's one"),
        2 => println!("it's two"),
        _ => println!("It's some other number"),
    }
}
```

那打印`It's some other number`。

记住匹配的规则:

- 你写下`match`，然后创建一个`{}`的代码块。
- 在左边写上*模式*，用`=>`胖箭头说明匹配时该怎么做。
- 每一行称为一个 "arm"。
- 在arm之间放一个逗号(不是分号)。

你可以用匹配来声明一个值。

```rust
fn main() {
    let my_number = 5;
    let second_number = match my_number {
        0 => 0,
        5 => 10,
        _ => 2,
    };
}
```

`second_number`将是10。你看到最后的分号了吗？那是因为，在match结束后，我们实际上告诉了编译器这个信息:`let second_number = 10;`


你也可以在更复杂的事情上进行匹配。你用一个元组来做。

```rust
fn main() {
    let sky = "cloudy";
    let temperature = "warm";

    match (sky, temperature) {
        ("cloudy", "cold") => println!("It's dark and unpleasant today"),
        ("clear", "warm") => println!("It's a nice day"),
        ("cloudy", "warm") => println!("It's dark but not bad"),
        _ => println!("Not sure what the weather is."),
    }
}
```

这打印了`It's dark but not bad`，因为它与`sky`和`temperature`的 "多云"和 "温暖"相匹配。

你甚至可以把`if`放在`match`里面。这就是所谓的 "match guard"。

```rust
fn main() {
    let children = 5;
    let married = true;

    match (children, married) {
        (children, married) if married == false => println!("Not married with {} children", children),
        (children, married) if children == 0 && married == true => println!("Married but no children"),
        _ => println!("Married? {}. Number of children: {}.", married, children),
    }
}
```

这将打印`Married? true. Number of children: 5.`

在一次匹配中，你可以随意使用 _ 。在这个关于颜色的匹配中，我们有三个颜色，但一次只能选中一个。

```rust
fn match_colours(rbg: (i32, i32, i32)) {
    match rbg {
        (r, _, _) if r < 10 => println!("Not much red"),
        (_, b, _) if b < 10 => println!("Not much blue"),
        (_, _, g) if g < 10 => println!("Not much green"),
        _ => println!("Each colour has at least 10"),
    }
}

fn main() {
    let first = (200, 0, 0);
    let second = (50, 50, 50);
    let third = (200, 50, 0);

    match_colours(first);
    match_colours(second);
    match_colours(third);

}
```

这个将打印:

```text
Not much blue
Each colour has at least 10
Not much green
```

这也说明了`match`语句的作用，因为在第一个例子中，它只打印了`Not much blue`。但是`first`也没有多少绿色。`match`语句总是在找到一个匹配项时停止，而不检查其他的。这就是一个很好的例子，代码编译得很好，但不是你想要的代码。

你可以创建一个非常大的 `match` 语句来解决这个问题，但是使用 `for` 循环可能更好。我们将很快讨论循环。

匹配必须返回相同的类型。所以你不能这样做:

```rust
fn main() {
    let my_number = 10;
    let some_variable = match my_number {
        10 => 8,
        _ => "Not ten", // ⚠️
    };
}
```

编译器告诉你:

```text
error[E0308]: `match` arms have incompatible types
  --> src\main.rs:17:14
   |
15 |       let some_variable = match my_number {
   |  _________________________-
16 | |         10 => 8,
   | |               - this is found to be of type `{integer}`
17 | |         _ => "Not ten",
   | |              ^^^^^^^^^ expected integer, found `&str`
18 | |     };
   | |_____- `match` arms have incompatible types
```

这样也不行，原因同上。

```rust
fn main() {
    let some_variable = if my_number == 10 { 8 } else { "something else "}; // ⚠️
}
```

但是这样就可以了，因为不是`match`，所以你每次都有不同的`let`语句。

```rust
fn main() {
    let my_number = 10;

    if my_number == 10 {
        let some_variable = 8;
    } else {
        let some_variable = "Something else";
    }
}
```

你也可以使用 `@` 给 `match` 表达式的值起一个名字，然后你就可以使用它。在这个例子中，我们在一个函数中匹配一个 `i32` 输入。如果是4或13，我们要在`println!`语句中使用这个数字。否则，我们不需要使用它。

```rust
fn match_number(input: i32) {
    match input {
    number @ 4 => println!("{} is an unlucky number in China (sounds close to 死)!", number),
    number @ 13 => println!("{} is unlucky in North America, lucky in Italy! In bocca al lupo!", number),
    _ => println!("Looks like a normal number"),
    }
}

fn main() {
    match_number(50);
    match_number(13);
    match_number(4);
}
```

这个打印:

```text
Looks like a normal number
13 is unlucky in North America, lucky in Italy! In bocca al lupo!
4 is an unlucky number in China (sounds close to 死)!
```

## 结构体

有了结构体，你可以创建自己的类型。在 Rust 中，你会一直使用结构体，因为它们非常方便。结构体是用关键字 `struct` 创建的。结构体的名称应该用UpperCamelCase(每个字用大写字母，不要用空格)。如果你用全小写的结构，编译器会告诉你。

有三种类型的结构。一种是 "单元结构"。单元的意思是 "没有任何东西"。对于一个单元结构，你只需要写名字和一个分号。

```rust
struct FileDirectory;
fn main() {}
```

接下来是一个元组结构，或者说是一个未命名结构。之所以是 "未命名"，是因为你只需要写类型，而不是字段名。当你需要一个简单的结构，并且不需要记住名字时，元组结构是很好的选择。

```rust
struct Colour(u8, u8, u8);

fn main() {
    let my_colour = Colour(50, 0, 50); // Make a colour out of RGB (red, green, blue)
    println!("The second part of the colour is: {}", my_colour.1);
}
```

这时打印出`The second part of the colour is: 0`。

第三种类型是命名结构。这可能是最常见的结构。在这个结构中，你在一个 `{}` 代码块中声明字段名和类型。请注意，在命名结构后面不要写分号，因为后面有一整个代码块。

```rust
struct Colour(u8, u8, u8); // Declare the same Colour tuple struct

struct SizeAndColour {
    size: u32,
    colour: Colour, // And we put it in our new named struct
}

fn main() {
    let my_colour = Colour(50, 0, 50);

    let size_and_colour = SizeAndColour {
        size: 150,
        colour: my_colour
    };
}
```

在一个命名结构中，你也可以用逗号来分隔字段。对于最后一个字段，你可以加一个逗号或不加--这取决于你。`SizeAndColour` 在 `colour` 后面有一个逗号。

```rust
struct Colour(u8, u8, u8); // Declare the same Colour tuple struct

struct SizeAndColour {
    size: u32,
    colour: Colour, // And we put it in our new named struct
}

fn main() {}
```

但你不需要它。但总是放一个逗号可能是个好主意，因为有时你会改变字段的顺序。

```rust
struct Colour(u8, u8, u8); // Declare the same Colour tuple struct

struct SizeAndColour {
    size: u32,
    colour: Colour // No comma here
}

fn main() {}
```

然后我们决定改变顺序...

```rust
struct SizeAndColour {
    colour: Colour // ⚠️ Whoops! Now this doesn't have a comma.
    size: u32,
}

fn main() {}
```

但无论哪种方式都不是很重要，所以你可以选择是否使用逗号。


我们创建一个`Country`结构来举例说明。`Country`结构有`population`、`capital`和`leader_name`三个字段。

```rust
struct Country {
    population: u32,
    capital: String,
    leader_name: String
}

fn main() {
    let population = 500_000;
    let capital = String::from("Elista");
    let leader_name = String::from("Batu Khasikov");

    let kalmykia = Country {
        population: population,
        capital: capital,
        leader_name: leader_name,
    };
}
```

你有没有注意到，我们把同样的东西写了两次？我们写了`population: population`、`capital: capital`和`leader_name: leader_name`。实际上，你不需要这样做:如果字段名和变量名是一样的，你就不用写两次。

```rust
struct Country {
    population: u32,
    capital: String,
    leader_name: String
}

fn main() {
    let population = 500_000;
    let capital = String::from("Elista");
    let leader_name = String::from("Batu Khasikov");

    let kalmykia = Country {
        population,
        capital,
        leader_name,
    };
}
```

## 枚举

`enum`是enumerations的简称。它们看起来与结构体非常相似，但又有所不同。这就是区别:

- 当你想要一个东西**和**另一个东西时，使用`struct`.
- 当你想要一个东西**或**另一个东西时，请使用 `enum`。

所以，结构体是用于**多个事物**在一起，而枚举则是用于**多个选择**在一起。


要声明一个枚举，请写`enum`，并使用一个包含选项的代码块，用逗号分隔。就像 `struct` 一样，最后一部分可以有逗号，也可以没有。我们将创建一个名为 `ThingsInTheSky` 的枚举。

```rust
enum ThingsInTheSky {
    Sun,
    Stars,
}

fn main() {}
```

这是一个枚举，因为你可以看到太阳，**或**星星:你必须选择一个。这些叫做**变体**。

```rust
// create the enum with two choices
enum ThingsInTheSky {
    Sun,
    Stars,
}

// With this function we can use an i32 to create ThingsInTheSky.
fn create_skystate(time: i32) -> ThingsInTheSky {
    match time {
        6..=18 => ThingsInTheSky::Sun, // Between 6 and 18 hours we can see the sun
        _ => ThingsInTheSky::Stars, // Otherwise, we can see stars
    }
}

// With this function we can match against the two choices in ThingsInTheSky.
fn check_skystate(state: &ThingsInTheSky) {
    match state {
        ThingsInTheSky::Sun => println!("I can see the sun!"),
        ThingsInTheSky::Stars => println!("I can see the stars!")
    }
}

fn main() {
    let time = 8; // it's 8 o'clock
    let skystate = create_skystate(time); // create_skystate returns a ThingsInTheSky
    check_skystate(&skystate); // Give it a reference so it can read the variable skystate
}
```

这将打印出`I can see the sun!`。

你也可以将数据添加到一个枚举中。

```rust
enum ThingsInTheSky {
    Sun(String), // Now each variant has a string
    Stars(String),
}

fn create_skystate(time: i32) -> ThingsInTheSky {
    match time {
        6..=18 => ThingsInTheSky::Sun(String::from("I can see the sun!")), // Write the strings here
        _ => ThingsInTheSky::Stars(String::from("I can see the stars!")),
    }
}

fn check_skystate(state: &ThingsInTheSky) {
    match state {
        ThingsInTheSky::Sun(description) => println!("{}", description), // Give the string the name description so we can use it
        ThingsInTheSky::Stars(n) => println!("{}", n), // Or you can name it n. Or anything else - it doesn't matter
    }
}

fn main() {
    let time = 8; // it's 8 o'clock
    let skystate = create_skystate(time); // create_skystate returns a ThingsInTheSky
    check_skystate(&skystate); // Give it a reference so it can read the variable skystate
}
```

这样打印出来的结果是一样的:`I can see the sun!`。

你也可以 "导入"一个枚举，这样你就不用打那么多字了。下面是一个例子，我们每次在心情上匹配时都要输入 `Mood::`。

```rust
enum Mood {
    Happy,
    Sleepy,
    NotBad,
    Angry,
}

fn match_mood(mood: &Mood) -> i32 {
    let happiness_level = match mood {
        Mood::Happy => 10, // Here we type Mood:: every time
        Mood::Sleepy => 6,
        Mood::NotBad => 7,
        Mood::Angry => 2,
    };
    happiness_level
}

fn main() {
    let my_mood = Mood::NotBad;
    let happiness_level = match_mood(&my_mood);
    println!("Out of 1 to 10, my happiness is {}", happiness_level);
}
```

它打印的是`Out of 1 to 10, my happiness is 7`。让我们导入，这样我们就可以少打点字了。要导入所有的东西，写`*`。注意:它和`*`的解引用键是一样的，但完全不同。

```rust
enum Mood {
    Happy,
    Sleepy,
    NotBad,
    Angry,
}

fn match_mood(mood: &Mood) -> i32 {
    use Mood::*; // We imported everything in Mood. Now we can just write Happy, Sleepy, etc.
    let happiness_level = match mood {
        Happy => 10, // We don't have to write Mood:: anymore
        Sleepy => 6,
        NotBad => 7,
        Angry => 2,
    };
    happiness_level
}

fn main() {
    let my_mood = Mood::Happy;
    let happiness_level = match_mood(&my_mood);
    println!("Out of 1 to 10, my happiness is {}", happiness_level);
}
```


`enum` 的部分也可以变成一个整数。这是因为 Rust 给 `enum` 的每个arm提供了一个以 0 开头的数字，供它自己使用。如果你的枚举中没有任何其他数据，你可以用它来做一些事情。

```rust
enum Season {
    Spring, // If this was Spring(String) or something it wouldn't work
    Summer,
    Autumn,
    Winter,
}

fn main() {
    use Season::*;
    let four_seasons = vec![Spring, Summer, Autumn, Winter];
    for season in four_seasons {
        println!("{}", season as u32);
    }
}
```

这个打印:

```text
0
1
2
3
```

不过如果你想的话，你可以给它一个不同的数字--Rust并不在意，可以用同样的方式来使用它。只需在你想要的变体上加一个 `=` 和你的数字。你不必给所有的都分配一个数字。但如果你不这样做，Rust就会从前一个arm加1来赋值给当前arm。

```rust
enum Star {
    BrownDwarf = 10,
    RedDwarf = 50,
    YellowStar = 100,
    RedGiant = 1000,
    DeadStar, // Think about this one. What number will it have?
}

fn main() {
    use Star::*;
    let starvec = vec![BrownDwarf, RedDwarf, YellowStar, RedGiant];
    for star in starvec {
        match star as u32 {
            size if size <= 80 => println!("Not the biggest star."), // Remember: size doesn't mean anything. It's just a name we chose so we can print it
            size if size >= 80 => println!("This is a good-sized star."),
            _ => println!("That star is pretty big!"),
        }
    }
    println!("What about DeadStar? It's the number {}.", DeadStar as u32);
}
```

这个打印:


```text
Not the biggest star.
Not the biggest star.
This is a good-sized star.
This is a good-sized star.
What about DeadStar? It's the number 1001.
```

`DeadStar`本来是4号，但现在是1001。

### 使用多种类型的枚举

你知道`Vec`、数组等中的元素都需要相同的类型(只有tuple不同)。但其实你可以用一个枚举来放不同的类型。想象一下，我们想有一个`Vec`，有`u32`或`i32`。当然，你可以创建一个`Vec<(u32, i32)>`(一个带有`(u32, i32)`元组的vec)，但是我们每次只想要一个。所以这里可以使用一个枚举。下面是一个简单的例子。

```rust
enum Number {
    U32(u32),
    I32(i32),
}

fn main() {}
```

所以有两个变体:`U32`变体里面有`u32`，`I32`变体里面有`i32`。`U32`和`I32`只是我们起的名字。它们可能是`UThirtyTwo`或`IThirtyTwo`或其他任何东西。

现在，如果我们把它们放到 `Vec` 中，我们就会有一个 `Vec<Number>`，编译器很高兴，因为都是同一个类型。编译器并不在乎我们有 `u32` 或 `i32`，因为它们都在一个叫做 `Number` 的单一类型里面。因为它是一个枚举，你必须选择一个，这就是我们想要的。我们将使用`.is_positive()`方法来挑选。如果是 `true`，那么我们将选择 `U32`，如果是 `false`，那么我们将选择 `I32`。

现在的代码是这样的。

```rust
enum Number {
    U32(u32),
    I32(i32),
}

fn get_number(input: i32) -> Number {
    let number = match input.is_positive() {
        true => Number::U32(input as u32), // change it to u32 if it's positive
        false => Number::I32(input), // otherwise just give the number because it's already i32
    };
    number
}


fn main() {
    let my_vec = vec![get_number(-800), get_number(8)];

    for item in my_vec {
        match item {
            Number::U32(number) => println!("It's a u32 with the value {}", number),
            Number::I32(number) => println!("It's an i32 with the value {}", number),
        }
    }
}
```

这就打印出了我们想看到的东西。

```text
It's an i32 with the value -800
It's a u32 with the value 8
```


## 循环

有了循环，你可以告诉 Rust 继续某事，直到你想让它停止。您使用 `loop` 来启动一个不会停止的循环，除非您告诉它何时`break`。

```rust
fn main() { // This program will never stop
    loop {

    }
}
```

所以，我们要告诉编译器什么时候能停止:

```rust
fn main() {
    let mut counter = 0; // set a counter to 0
    loop {
        counter +=1; // increase the counter by 1
        println!("The counter is now: {}", counter);
        if counter == 5 { // stop when counter == 5
            break;
        }
    }
}
```

这将打印:

```text
The counter is now: 1
The counter is now: 2
The counter is now: 3
The counter is now: 4
The counter is now: 5
```

如果你在一个循环里面有一个循环，你可以给它们命名。有了名字，你可以告诉 Rust 要从哪个循环中 `break` 出来。使用 `'` (称为 "tick") 和 `:` 来给它命名。

```rust
fn main() {
    let mut counter = 0;
    let mut counter2 = 0;
    println!("Now entering the first loop.");

    'first_loop: loop {
        // Give the first loop a name
        counter += 1;
        println!("The counter is now: {}", counter);
        if counter > 9 {
            // Starts a second loop inside this loop
            println!("Now entering the second loop.");

            'second_loop: loop {
                // now we are inside 'second_loop
                println!("The second counter is now: {}", counter2);
                counter2 += 1;
                if counter2 == 3 {
                    break 'first_loop; // Break out of 'first_loop so we can exit the program
                }
            }
        }
    }
}
```

这将打印:

```text
Now entering the first loop.
The counter is now: 1
The counter is now: 2
The counter is now: 3
The counter is now: 4
The counter is now: 5
The counter is now: 6
The counter is now: 7
The counter is now: 8
The counter is now: 9
The counter is now: 10
Now entering the second loop.
The second counter is now: 0
The second counter is now: 1
The second counter is now: 2
```

`while`循环是指在某件事情还在`true`时继续的循环。每一次循环，Rust 都会检查它是否仍然是 `true`。如果变成`false`，Rust会停止循环。

```rust
fn main() {
    let mut counter = 0;

    while counter < 5 {
        counter +=1;
        println!("The counter is now: {}", counter);
    }
}
```

`for`循环可以让你告诉Rust每次要做什么。但是在 `for` 循环中，循环会在一定次数后停止。`for`循环经常使用**范围**。你使用 `..` 和 `..=` 来创建一个范围。

- `..`创建一个**排他的**范围:`0..3`创建了`0, 1, 2`.
- `..=`创建一个**包含的**范围: `0..=3`创建`0, 1, 2`。`0..=3` = `0, 1, 2, 3`.

```rust
fn main() {
    for number in 0..3 {
        println!("The number is: {}", number);
    }

    for number in 0..=3 {
        println!("The next number is: {}", number);
    }
}
```

这个将打印:

```text
The number is: 0
The number is: 1
The number is: 2
The next number is: 0
The next number is: 1
The next number is: 2
The next number is: 3
```

同时注意到，`number`成为0..3的变量名。我们可以把它叫做 `n`，或者 `ntod_het___hno_f`，或者任何名字。然后，我们可以在`println!`中使用这个名字。

如果你不需要变量名，就用`_`。

```rust
fn main() {
    for _ in 0..3 {
        println!("Printing the same thing three times");
    }
}
```

这个打印:

```text
Printing the same thing three times
Printing the same thing three times
Printing the same thing three times
```

因为我们每次都没有给它任何数字来打印。

而实际上，如果你给了一个变量名却不用，Rust会告诉你:

```rust
fn main() {
    for number in 0..3 {
        println!("Printing the same thing three times");
    }
}
```

这打印的内容和上面一样。程序编译正常，但Rust会提醒你没有使用`number`:

```text
warning: unused variable: `number`
 --> src\main.rs:2:9
  |
2 |     for number in 0..3 {
  |         ^^^^^^ help: if this is intentional, prefix it with an underscore: `_number`
```

Rust 建议写 `_number` 而不是 `_`。在变量名前加上 `_` 意味着 "也许我以后会用到它"。但是只用`_`意味着 "我根本不关心这个变量"。所以，如果你以后会使用它们，并且不想让编译器告诉你，你可以在变量名前面加上`_`。

你也可以用`break`来返回一个值。
 你把值写在 `break` 之后，并使用 `;`。下面是一个用 `loop` 和一个断点给出 `my_number` 值的例子。

```rust
fn main() {
    let mut counter = 5;
    let my_number = loop {
        counter +=1;
        if counter % 53 == 3 {
            break counter;
        }
    };
    println!("{}", my_number);
}
```

这时打印出`56`。`break counter;`的意思是 "中断并返回计数器的值"。而且因为整个块以`let`开始，所以`my_number`得到值。

现在我们知道了如何使用循环，这里有一个更好的解决方案来解决我们之前的颜色 "匹配"问题。这是一个更好的解决方案，因为我们要比较所有的东西，而 "for"循环会查看每一项。

```rust
fn match_colours(rbg: (i32, i32, i32)) {
    println!("Comparing a colour with {} red, {} blue, and {} green:", rbg.0, rbg.1, rbg.2);
    let new_vec = vec![(rbg.0, "red"), (rbg.1, "blue"), (rbg.2, "green")]; // Put the colours in a vec. Inside are tuples with the colour names
    let mut all_have_at_least_10 = true; // Start with true. We will set it to false if one colour is less than 10
    for item in new_vec {
        if item.0 < 10 {
            all_have_at_least_10 = false; // Now it's false
            println!("Not much {}.", item.1) // And we print the colour name.
        }
    }
    if all_have_at_least_10 { // Check if it's still true, and print if true
        println!("Each colour has at least 10.")
    }
    println!(); // Add one more line
}

fn main() {
    let first = (200, 0, 0);
    let second = (50, 50, 50);
    let third = (200, 50, 0);

    match_colours(first);
    match_colours(second);
    match_colours(third);
}
```

这个打印:

```text
Comparing a colour with 200 red, 0 blue, and 0 green:
Not much blue.
Not much green.

Comparing a colour with 50 red, 50 blue, and 50 green:
Each colour has at least 10.

Comparing a colour with 200 red, 50 blue, and 0 green:
Not much green.
```

## 实现结构体和枚举

在这里你可以开始赋予你的结构体和枚举一些真正的力量。要调用 `struct` 或 `enum` 上的函数，请使用 `impl` 块。这些函数被称为**方法**。`impl`块中有两种方法。

- 方法：这些方法取**self**（或 **&self** 或 **&mut self** ）。常规方法使用"."（一个句号）。`.clone()`是一个常规方法的例子。
- 关联函数（在某些语言中被称为 "静态 "方法）：这些函数不使用self。关联的意思是 "与之相关"。它们的书写方式不同，使用`::`。`String::from()`是一个关联函数，`Vec::new()`也是。你看到的关联函数最常被用来创建新的变量。

在我们的例子中，我们将创建Animal并打印它们。

对于新的`struct`或`enum`，如果你想使用`{:?}`来打印，你需要给它**Debug**，所以我们将这样做:如果你在结构体或枚举上面写了`#[derive(Debug)]`，那么你就可以用`{:?}`来打印。这些带有`#[]`的信息被称为**属性**。你有时可以用它们来告诉编译器给你的结构体一个能力，比如`Debug`。属性有很多，我们以后会学习它们。但是`derive`可能是最常见的，你经常在结构体和枚举上面看到它。

```rust
#[derive(Debug)]
struct Animal {
    age: u8,
    animal_type: AnimalType,
}

#[derive(Debug)]
enum AnimalType {
    Cat,
    Dog,
}

impl Animal {
    fn new() -> Self {
        // Self means Animal.
        //You can also write Animal instead of Self

        Self {
            // When we write Animal::new(), we always get a cat that is 10 years old
            age: 10,
            animal_type: AnimalType::Cat,
        }
    }

    fn change_to_dog(&mut self) { // because we are inside Animal, &mut self means &mut Animal
                                  // use .change_to_dog() to change the cat to a dog
                                  // with &mut self we can change it
        println!("Changing animal to dog!");
        self.animal_type = AnimalType::Dog;
    }

    fn change_to_cat(&mut self) {
        // use .change_to_cat() to change the dog to a cat
        // with &mut self we can change it
        println!("Changing animal to cat!");
        self.animal_type = AnimalType::Cat;
    }

    fn check_type(&self) {
        // we want to read self
        match self.animal_type {
            AnimalType::Dog => println!("The animal is a dog"),
            AnimalType::Cat => println!("The animal is a cat"),
        }
    }
}



fn main() {
    let mut new_animal = Animal::new(); // Associated function to create a new animal
                                        // It is a cat, 10 years old
    new_animal.check_type();
    new_animal.change_to_dog();
    new_animal.check_type();
    new_animal.change_to_cat();
    new_animal.check_type();
}
```

这个打印:

```text
The animal is a cat
Changing animal to dog!
The animal is a dog
Changing animal to cat!
The animal is a cat
```


记住，Self(类型Self)和self(变量self)是缩写。(缩写=简写方式)

所以，在我们的代码中，Self = Animal。另外，`fn change_to_dog(&mut self)`的意思是`fn change_to_dog(&mut Animal)`。

下面再举一个小例子。这次我们将在`enum`上使用`impl`。

```rust
enum Mood {
    Good,
    Bad,
    Sleepy,
}

impl Mood {
    fn check(&self) {
        match self {
            Mood::Good => println!("Feeling good!"),
            Mood::Bad => println!("Eh, not feeling so good"),
            Mood::Sleepy => println!("Need sleep NOW"),
        }
    }
}

fn main() {
    let my_mood = Mood::Sleepy;
    my_mood.check();
}
```

打印出`Need sleep NOW`。

## 解构

我们再来看一些解构。你可以通过使用`let`倒过来从一个结构体或枚举中获取值。我们了解到这是`destructuring`，因为你得到的变量不是结构体的一部分。现在你分别得到了它们的值。首先是一个简单的例子。

```rust
struct Person { // make a simple struct for a person
    name: String,
    real_name: String,
    height: u8,
    happiness: bool
}

fn main() {
    let papa_doc = Person { // create variable papa_doc
        name: "Papa Doc".to_string(),
        real_name: "Clarence".to_string(),
        height: 170,
        happiness: false
    };

    let Person { // destructure papa_doc
        name: a,
        real_name: b,
        height: c,
        happiness: d
    } = papa_doc;

    println!("They call him {} but his real name is {}. He is {} cm tall and is he happy? {}", a, b, c, d);
}
```

这个打印:`They call him Papa Doc but his real name is Clarence. He is 170 cm tall and is he happy? false`

你可以看到，这是倒过来的。首先我们说`let papa_doc = Person { fields }`来创建结构。然后我们说 `let Person { fields } = papa_doc` 来解构它。

你不必写`name: a`--你可以直接写`name`。但这里我们写 `name: a` 是因为我们想使用一个名字为 `a` 的变量。

现在再举一个更大的例子。在这个例子中，我们有一个 `City` 结构。我们给它一个`new`函数来创建它。然后我们有一个 `process_city_values` 函数来处理这些值。在函数中，我们只是创建了一个 `Vec`，但你可以想象，我们可以在解构它之后做更多的事情。

```rust
struct City {
    name: String,
    name_before: String,
    population: u32,
    date_founded: u32,
}

impl City {
    fn new(name: String, name_before: String, population: u32, date_founded: u32) -> Self {
        Self {
            name,
            name_before,
            population,
            date_founded,
        }
    }
}

fn process_city_values(city: &City) {
    let City {
        name,
        name_before,
        population,
        date_founded,
    } = city;
        // now we have the values to use separately
    let two_names = vec![name, name_before];
    println!("The city's two names are {:?}", two_names);
}

fn main() {
    let tallinn = City::new("Tallinn".to_string(), "Reval".to_string(), 426_538, 1219);
    process_city_values(&tallinn);
}
```

这将打印出`The city's two names are ["Tallinn", "Reval"]`。


## 引用和点运算符

我们了解到，当你有一个引用时，你需要使用`*`来获取值。引用是一种不同的类型，所以这是无法运行的:

```rust
fn main() {
    let my_number = 9;
    let reference = &my_number;

    println!("{}", my_number == reference); // ⚠️
}
```

编译器打印。

```text
error[E0277]: can't compare `{integer}` with `&{integer}`
 --> src\main.rs:5:30
  |
5 |     println!("{}", my_number == reference);
  |                              ^^ no implementation for `{integer} == &{integer}`
```

所以我们把第5行改成`println!("{}", my_number == *reference);`，现在打印的是`true`，因为现在是`i32` == `i32`，而不是`i32` == `&i32`。这就是所谓的解引用。

但是当你使用一个方法时，Rust会为你解除引用。方法中的 `.` 被称为点运算符，它可以免费进行递归。

首先，让我们创建一个有一个 `u8` 字段的结构。然后，我们将对它进行引用，并尝试进行比较。它将无法工作。

```rust
struct Item {
    number: u8,
}

fn main() {
    let item = Item {
        number: 8,
    };

    let reference_number = &item.number; // reference number type is &u8

    println!("{}", reference_number == 8); // ⚠️ &u8 and u8 cannot be compared
}
```

为了让它工作，我们需要取消定义。`println!("{}", *reference_number == 8);`.

但如果使用点运算符，我们不需要`*`。例如

```rust
struct Item {
    number: u8,
}

fn main() {
    let item = Item {
        number: 8,
    };

    let reference_item = &item;

    println!("{}", reference_item.number == 8); // we don't need to write *reference_item.number
}
```

现在让我们为 `Item` 创建一个方法，将 `number` 与另一个数字进行比较。我们不需要在任何地方使用 `*`。

```rust
struct Item {
    number: u8,
}

impl Item {
    fn compare_number(&self, other_number: u8) { // takes a reference to self
        println!("Are {} and {} equal? {}", self.number, other_number, self.number == other_number);
            // We don't need to write *self.number
    }
}

fn main() {
    let item = Item {
        number: 8,
    };

    let reference_item = &item; // This is type &Item
    let reference_item_two = &reference_item; // This is type &&Item

    item.compare_number(8); // the method works
    reference_item.compare_number(8); // it works here too
    reference_item_two.compare_number(8); // and here

}
```

所以只要记住:当你使用`.`运算符时，你不需要担心`*`。


## 泛型

在函数中，你要写出采取什么类型作为输入。

```rust
fn return_number(number: i32) -> i32 {
    println!("Here is your number.");
    number
}

fn main() {
    let number = return_number(5);
}
```

但是如果你想用的不仅仅是`i32`呢？你可以用泛型来解决。Generics的意思是 "也许是一种类型，也许是另一种类型"。

对于泛型，你可以使用角括号，里面加上类型，像这样。`<T>` 这意味着 "任何类型你都可以放入函数中" 通常情况下，generics使用一个大写字母的类型(T、U、V等)，尽管你不必只使用一个字母。

这就是你如何改变函数使其通用的方法。

```rust
fn return_number<T>(number: T) -> T {
    println!("Here is your number.");
    number
}

fn main() {
    let number = return_number(5);
}
```

重要的部分是函数名后的`<T>`。如果没有这个，Rust会认为T是一个具体的(具体的=不是通用的)类型。
 如`String`或`i8`。

如果我们写出一个类型名，这就更容易理解了。看看我们把 `T` 改成 `MyType` 会发生什么。

```rust
fn return_number(number: MyType) -> MyType { // ⚠️
    println!("Here is your number.");
    number
}
```

大家可以看到，`MyType`是具体的，不是通用的。所以我们需要写这个，所以现在就可以了。

```rust
fn return_number<MyType>(number: MyType) -> MyType {
    println!("Here is your number.");
    number
}

fn main() {
    let number = return_number(5);
}
```

所以单字母`T`是人的眼睛，但函数名后面的部分是编译器的 "眼睛"。没有了它，就不通用了。

现在我们再回到类型`T`，因为Rust代码通常使用`T`。

你会记得Rust中有些类型是**Copy**，有些是**Clone**，有些是**Display**，有些是**Debug**，等等。用**Debug**，我们可以用`{:?}`来打印。所以现在大家可以看到，我们如果要打印`T`就有问题了。

```rust
fn print_number<T>(number: T) {
    println!("Here is your number: {:?}", number); // ⚠️
}

fn main() {
    print_number(5);
}
```

`print_number`需要**Debug**打印`number`，但是`T`与`Debug`是一个类型吗？也许不是。也许它没有`#[derive(Debug)]`，谁知道呢？编译器也不知道，所以它给出了一个错误。

```text
error[E0277]: `T` doesn't implement `std::fmt::Debug`
  --> src\main.rs:29:43
   |
29 |     println!("Here is your number: {:?}", number);
   |                                           ^^^^^^ `T` cannot be formatted using `{:?}` because it doesn't implement `std::fmt::Debug`
```

T没有实现**Debug**。那么我们是否要为T实现Debug呢？不，因为我们不知道T是什么。但是我们可以告诉函数。"别担心，因为任何T类型的函数都会有Debug"

```rust
use std::fmt::Debug; // Debug is located at std::fmt::Debug. So now we can just write 'Debug'.

fn print_number<T: Debug>(number: T) { // <T: Debug> is the important part
    println!("Here is your number: {:?}", number);
}

fn main() {
    print_number(5);
}
```

所以现在编译器知道:"好的，这个类型T要有Debug"。现在代码工作了，因为`i32`有Debug。现在我们可以给它很多类型。`String`, `&str`, 等等，因为它们都有Debug.

现在我们可以创建一个结构，并用#[derive(Debug)]给它Debug，所以现在我们也可以打印它。我们的函数可以取`i32`，Animal结构等。

```rust
use std::fmt::Debug;

#[derive(Debug)]
struct Animal {
    name: String,
    age: u8,
}

fn print_item<T: Debug>(item: T) {
    println!("Here is your item: {:?}", item);
}

fn main() {
    let charlie = Animal {
        name: "Charlie".to_string(),
        age: 1,
    };

    let number = 55;

    print_item(charlie);
    print_item(number);
}
```

这个打印:

```text
Here is your item: Animal { name: "Charlie", age: 1 }
Here is your item: 55
```

有时候，我们在一个通用函数中需要不止一个类型。我们必须写出每个类型的名称，并考虑如何使用它。在这个例子中，我们想要两个类型。首先我们要打印一个类型为T的语句。用`{}`打印比较好，所以我们会要求用`Display`来打印`T`。

其次是类型U，`num_1`和`num_2`这两个变量的类型为U(U是某种数字)。我们想要比较它们，所以我们需要`PartialOrd`。这个特性让我们可以使用`<`、`>`、`==`等。我们也想打印它们，所以我们也需要`Display`来打印`U`。

```rust
use std::fmt::Display;
use std::cmp::PartialOrd;

fn compare_and_display<T: Display, U: Display + PartialOrd>(statement: T, num_1: U, num_2: U) {
    println!("{}! Is {} greater than {}? {}", statement, num_1, num_2, num_1 > num_2);
}

fn main() {
    compare_and_display("Listen up!", 9, 8);
}
```

这就打印出了`Listen up!! Is 9 greater than 8? true`。

所以`fn compare_and_display<T: Display, U: Display + PartialOrd>(statement: T, num_1: U, num_2: U)`说。

- 函数名称是`compare_and_display`,
- 第一个类型是T，它是通用的。它必须是一个可以用{}打印的类型。
- 下一个类型是U，它是通用的。它必须是一个可以用{}打印的类型。另外，它必须是一个可以比较的类型(使用 `>`、`<` 和 `==`)。

现在我们可以给`compare_and_display`不同的类型。`statement`可以是一个`String`，一个`&str`，任何有Display的类型。

为了让通用函数更容易读懂，我们也可以这样写，在代码块之前就写上`where`。

```rust
use std::cmp::PartialOrd;
use std::fmt::Display;

fn compare_and_display<T, U>(statement: T, num_1: U, num_2: U)
where
    T: Display,
    U: Display + PartialOrd,
{
    println!("{}! Is {} greater than {}? {}", statement, num_1, num_2, num_1 > num_2);
}

fn main() {
    compare_and_display("Listen up!", 9, 8);
}
```

当你有很多通用类型时，使用`where`是一个好主意。

还要注意。

- 如果你有一个类型T和另一个类型T，它们必须是相同的。
- 如果你有一个类型T和另一个类型U，它们可以是不同的。但它们也可以是相同的。

比如说

```rust
use std::fmt::Display;

fn say_two<T: Display, U: Display>(statement_1: T, statement_2: U) { // Type T needs Display, type U needs Display
    println!("I have two things to say: {} and {}", statement_1, statement_2);
}

fn main() {

    say_two("Hello there!", String::from("I hate sand.")); // Type T is a &str, but type U is a String.
    say_two(String::from("Where is Padme?"), String::from("Is she all right?")); // Both types are String.
}
```

这个打印:

```text
I have two things to say: Hello there! and I hate sand.
I have two things to say: Where is Padme? and Is she all right?
```

## Option和Result

我们现在理解了枚举和泛型，所以我们可以理解`Option`和`Result`。Rust使用这两个枚举来使代码更安全。

我们将从`Option`开始。

### Option

当你有一个可能存在，也可能不存在的值时，你就用`Option`。当一个值存在的时候就是`Some(value)`，不存在的时候就是`None`，下面是一个坏代码的例子，可以用`Option`来改进。

```rust
    // ⚠️
fn take_fifth(value: Vec<i32>) -> i32 {
    value[4]
}

fn main() {
    let new_vec = vec![1, 2];
    let index = take_fifth(new_vec);
}
```

当我们运行这段代码时，它崩溃。以下是信息。

```text
thread 'main' panicked at 'index out of bounds: the len is 2 but the index is 4', src\main.rs:34:5
```

崩溃的意思是，程序在问题发生之前就停止了。Rust看到函数想要做一些不可能的事情，就会停止。它 "解开堆栈"(从堆栈中取值)，并告诉你 "对不起，我不能这样做"。

所以现在我们将返回类型从`i32`改为`Option<i32>`。这意味着 "如果有的话给我一个`Some(i32)`，如果没有的话给我一个`None`"。我们说`i32`是 "包"在一个`Option`里面，也就是说它在一个`Option`里面。你必须做一些事情才能把这个值弄出来。

```rust
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 { // .len() gives the length of the vec.
                         // It must be at least 5.
        None
    } else {
        Some(value[4])
    }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    println!("{:?}, {:?}", take_fifth(new_vec), take_fifth(bigger_vec));
}
```

这个打印的是`None, Some(5)`。这下好了，因为现在我们再也不崩溃了。但是我们如何得到5的值呢？

我们可以用 `.unwrap()` 在一个Option中获取值，但要小心 `.unwrap()`。这就像拆礼物一样:也许里面有好东西，也许里面有一条愤怒的蛇。只有在你确定的情况下，你才会想要`.unwrap()`。如果你拆开一个`None`的值，程序就会崩溃。

```rust
// ⚠️
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 {
        None
    } else {
        Some(value[4])
    }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    println!("{:?}, {:?}",
        take_fifth(new_vec).unwrap(), // this one is None. .unwrap() will panic!
        take_fifth(bigger_vec).unwrap()
    );
}
```

消息是: 
```text
thread 'main' panicked at 'called `Option::unwrap()` on a `None` value', src\main.rs:14:9
```

但我们不需要使用`.unwrap()`。我们可以使用`match`。那么我们就可以把我们有`Some`的值打印出来，如果有`None`的值就不要碰。比如说

```rust
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 {
        None
    } else {
        Some(value[4])
    }
}

fn handle_option(my_option: Vec<Option<i32>>) {
  for item in my_option {
    match item {
      Some(number) => println!("Found a {}!", number),
      None => println!("Found a None!"),
    }
  }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    let mut option_vec = Vec::new(); // Make a new vec to hold our options
                                     // The vec is type: Vec<Option<i32>>. That means a vec of Option<i32>.

    option_vec.push(take_fifth(new_vec)); // This pushes "None" into the vec
    option_vec.push(take_fifth(bigger_vec)); // This pushes "Some(5)" into the vec

    handle_option(option_vec); // handle_option looks at every option in the vec.
                               // It prints the value if it is Some. It doesn't touch it if it is None.
}
```

这个打印:

```text
Found a None!
Found a 5!
```


因为我们知道泛型，所以我们能够读懂`Option`的代码。它看起来是这样的:

```rust
enum Option<T> {
    None,
    Some(T),
}

fn main() {}
```

要记住的重要一点是:有了`Some`，你就有了一个类型为`T`的值(任何类型)。还要注意的是，`enum`名字后面的角括号围绕着`T`是告诉编译器它是通用的。它没有`Display`这样的trait或任何东西来限制它，所以它可以是任何东西。但是对于`None`，你什么都没有。

所以在`match`语句中，对于Option，你不能说。

```rust
// 🚧
Some(value) => println!("The value is {}", value),
None(value) => println!("The value is {}", value),
```

因为`None`只是`None`。

当然，还有更简单的方法来使用Option。在这段代码中，我们将使用一个叫做 `.is_some()` 的方法来告诉我们是否是 `Some`。(是的，还有一个叫做`.is_none()`的方法。)在这个更简单的方法中，我们不需要`handle_option()`了。我们也不需要Option的vec了。

```rust
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 {
        None
    } else {
        Some(value[4])
    }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    let vec_of_vecs = vec![new_vec, bigger_vec];
    for vec in vec_of_vecs {
        let inside_number = take_fifth(vec);
        if inside_number.is_some() {
            // .is_some() returns true if we get Some, false if we get None
            println!("We got: {}", inside_number.unwrap()); // now it is safe to use .unwrap() because we already checked
        } else {
            println!("We got nothing.");
        }
    }
}
```

这个将打印:

```text
We got nothing.
We got: 5
```

### Result

Result和Option类似，但这里的区别是。

- Option大约是`Some`或`None`(有值或无值)。
- Result大约是`Ok`或`Err`(还好的结果，或错误的结果)。

所以，`Option`是如果你在想:"也许会有，也许不会有。"也许会有一些东西，也许不会有。" 但`Result`是如果你在想: "也许会失败"

比较一下，这里是Option和Result的签名。

```rust
enum Option<T> {
    None,
    Some(T),
}

enum Result<T, E> {
    Ok(T),
    Err(E),
}

fn main() {}
```

所以Result在 "Ok "里面有一个值，在 "Err "里面有一个值。这是因为错误通常包含描述错误的信息。

`Result<T, E>`的意思是你要想好`Ok`要返回什么，`Err`要返回什么。其实，你可以决定任何事情。甚至这个也可以。

```rust
fn check_error() -> Result<(), ()> {
    Ok(())
}

fn main() {
    check_error();
}
```

`check_error`说 "如果得到`Ok`就返回`()`，如果得到`Err`就返回`()`"。然后我们用`()`返回`Ok`。

编译器给了我们一个有趣的警告。

```text
warning: unused `std::result::Result` that must be used
 --> src\main.rs:6:5
  |
6 |     check_error();
  |     ^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_must_use)]` on by default
  = note: this `Result` may be an `Err` variant, which should be handled
```

这是真的:我们只返回了`Result`，但它可能是一个`Err`。所以让我们稍微处理一下这个错误，尽管我们仍然没有真正做任何事情。

```rust
fn give_result(input: i32) -> Result<(), ()> {
    if input % 2 == 0 {
        return Ok(())
    } else {
        return Err(())
    }
}

fn main() {
    if give_result(5).is_ok() {
        println!("It's okay, guys")
    } else {
        println!("It's an error, guys")
    }
}
```

打印出`It's an error, guys`。所以我们只是处理了第一个错误。

记住，轻松检查的四种方法是`.is_some()`、`is_none()`、`is_ok()`和`is_err()`。


有时，一个带有Result的函数会用`String`来表示`Err`的值。这不是最好的方法，但比我们目前所做的要好一些。

```rust
fn check_if_five(number: i32) -> Result<i32, String> {
    match number {
        5 => Ok(number),
        _ => Err("Sorry, the number wasn't five.".to_string()), // This is our error message
    }
}

fn main() {
    let mut result_vec = Vec::new(); // Create a new vec for the results

    for number in 2..7 {
        result_vec.push(check_if_five(number)); // push each result into the vec
    }

    println!("{:?}", result_vec);
}
```

我们的Vec打印:

```text
[Err("Sorry, the number wasn\'t five."), Err("Sorry, the number wasn\'t five."), Err("Sorry, the number wasn\'t five."), Ok(5),
Err("Sorry, the number wasn\'t five.")]
```

就像Option一样，在`Err`上用`.unwrap()`就会崩溃。

```rust
    // ⚠️
fn main() {
    let error_value: Result<i32, &str> = Err("There was an error"); // Create a Result that is already an Err
    println!("{}", error_value.unwrap()); // Unwrap it
}
```

程序崩溃，打印。

```text
thread 'main' panicked at 'called `Result::unwrap()` on an `Err` value: "There was an error"', src\main.rs:30:20
```

这些信息可以帮助你修正你的代码。`src\main.rs:30:20`的意思是 "在目录src的main.rs内，第30行和第20列"。所以你可以去那里查看你的代码并修复问题。

你也可以创建自己的错误类型，标准库中的Result函数和其他人的代码通常都会这样做。例如，标准库中的这个函数。

```rust
// 🚧
pub fn from_utf8(vec: Vec<u8>) -> Result<String, FromUtf8Error>
```

这个函数接收一个字节向量(`u8`)，并尝试创建一个`String`，所以Result的成功情况是`String`，错误情况是`FromUtf8Error`。你可以给你的错误类型起任何你想要的名字。

使用 `match` 与 `Option` 和 `Result` 有时需要很多代码。例如，`.get()` 方法在 `Vec` 上返回 `Option`。

```rust
fn main() {
    let my_vec = vec![2, 3, 4];
    let get_one = my_vec.get(0); // 0 to get the first number
    let get_two = my_vec.get(10); // Returns None
    println!("{:?}", get_one);
    println!("{:?}", get_two);
}
```

此打印

```text
Some(2)
None
```

所以现在我们可以匹配得到数值。让我们使用0到10的范围，看看是否符合`my_vec`中的数字。

```rust
fn main() {
    let my_vec = vec![2, 3, 4];

    for index in 0..10 {
      match my_vec.get(index) {
        Some(number) => println!("The number is: {}", number),
        None => {}
      }
    }
}
```

这是好的，但是我们对`None`不做任何处理，因为我们不关心。这里我们可以用`if let`把代码变小。`if let`的意思是 "符合就做，不符合就不做"。`if let`是在你不要求对所有的东西都匹配的时候使用。

```rust
fn main() {
    let my_vec = vec![2, 3, 4];

    for index in 0..10 {
      if let Some(number) = my_vec.get(index) {
        println!("The number is: {}", number);
      }
    }
}
```

**重要的是要记住**。`if let Some(number) = my_vec.get(index)`的意思是 "如果你从`my_vec.get(index)`得到`Some(number)`"。

另外注意:它使用的是一个`=`。它不是一个布尔值。

`while let`就像`if let`的一个while循环。想象一下，我们有这样的气象站数据。

```text
["Berlin", "cloudy", "5", "-7", "78"]
["Athens", "sunny", "not humid", "20", "10", "50"]
```

我们想得到数字，但不想得到文字。对于数字，我们可以使用一个叫做 `parse::<i32>()` 的方法。`parse()`是方法，`::<i32>`是类型。它将尝试把 `&str` 变成 `i32`，如果可以的话就把它给我们。它返回一个 `Result`，因为它可能无法工作(比如你想让它解析 "Billybrobby"--那不是一个数字)。

我们还将使用 `.pop()`。这将从向量中取出最后一项。

```rust
fn main() {
    let weather_vec = vec![
        vec!["Berlin", "cloudy", "5", "-7", "78"],
        vec!["Athens", "sunny", "not humid", "20", "10", "50"],
    ];
    for mut city in weather_vec {
        println!("For the city of {}:", city[0]); // In our data, every first item is the city name
        while let Some(information) = city.pop() {
            // This means: keep going until you can't pop anymore
            // When the vector reaches 0 items, it will return None
            // and it will stop.
            if let Ok(number) = information.parse::<i32>() {
                // Try to parse the variable we called information
                // This returns a result. If it's Ok(number), it will print it
                println!("The number is: {}", number);
            }  // We don't write anything here because we do nothing if we get an error. Throw them all away
        }
    }
}
```

这将打印:

```text
For the city of Berlin:
The number is: 78
The number is: -7
The number is: 5
For the city of Athens:
The number is: 50
The number is: 10
The number is: 20
```

## 其他集合类型

Rust还有很多集合类型。你可以在标准库中的 https://doc.rust-lang.org/beta/std/collections/ 看到它们。那个页面对为什么要使用一种类型有很好的解释，所以如果你不知道你想要什么类型，就去那里。这些集合都在标准库的`std::collections`里面。使用它们的最好方法是使用 `use` 语句。
 就像我们的`enums`一样。我们将从`HashMap`开始，这是很常见的。

### HashMap和BTreeMap

HashMap是由*keys*和*values*组成的集合。你使用键来查找与键匹配的值。你可以只用`HashMap::new()`创建一个新的`HashMap`，并使用`.insert(key, value)`来插入元素。

`HashMap`是没有顺序的，所以如果你把`HashMap`中的每一个键都打印在一起，可能会打印出不同的结果。我们可以在一个例子中看到这一点。

```rust
use std::collections::HashMap; // This is so we can just write HashMap instead of std::collections::HashMap every time

struct City {
    name: String,
    population: HashMap<u32, u32>, // This will have the year and the population for the year
}

fn main() {

    let mut tallinn = City {
        name: "Tallinn".to_string(),
        population: HashMap::new(), // So far the HashMap is empty
    };

    tallinn.population.insert(1372, 3_250); // insert three dates
    tallinn.population.insert(1851, 24_000);
    tallinn.population.insert(2020, 437_619);


    for (year, population) in tallinn.population { // The HashMap is HashMap<u32, u32> so it returns a two items each time
        println!("In the year {} the city of {} had a population of {}.", year, tallinn.name, population);
    }
}
```

这个打印:

```text
In the year 1372 the city of Tallinn had a population of 3250.
In the year 2020 the city of Tallinn had a population of 437619.
In the year 1851 the city of Tallinn had a population of 24000.
```

或者可能会打印。

```text
In the year 1851 the city of Tallinn had a population of 24000.
In the year 2020 the city of Tallinn had a population of 437619.
In the year 1372 the city of Tallinn had a population of 3250.
```

你可以看到，它不按顺序排列。

如果你想要一个可以排序的`HashMap`，你可以用`BTreeMap`。其实它们之间是非常相似的，所以我们可以快速的把我们的`HashMap`改成`BTreeMap`来看看。大家可以看到，这几乎是一样的代码。

```rust
use std::collections::BTreeMap; // Just change HashMap to BTreeMap

struct City {
    name: String,
    population: BTreeMap<u32, u32>, // Just change HashMap to BTreeMap
}

fn main() {

    let mut tallinn = City {
        name: "Tallinn".to_string(),
        population: BTreeMap::new(), // Just change HashMap to BTreeMap
    };

    tallinn.population.insert(1372, 3_250);
    tallinn.population.insert(1851, 24_000);
    tallinn.population.insert(2020, 437_619);

    for (year, population) in tallinn.population {
        println!("In the year {} the city of {} had a population of {}.", year, tallinn.name, population);
    }
}
```

现在会一直打印。

```text
In the year 1372 the city of Tallinn had a population of 3250.
In the year 1851 the city of Tallinn had a population of 24000.
In the year 2020 the city of Tallinn had a population of 437619.
```

现在我们再来看看`HashMap`。

只要把键放在`[]`的方括号里，就可以得到`HashMap`的值。在接下来的这个例子中，我们将带出`Bielefeld`这个键的值，也就是`Germany`。但是要注意，因为如果没有键，程序会崩溃。比如你写了`println!("{:?}", city_hashmap["Bielefeldd"]);`，那么就会崩溃，因为`Bielefeldd`不存在。

如果你不确定会有一个键，你可以使用`.get()`，它返回一个`Option`。如果它存在，将是`Some(value)`，如果不存在，你将得到`None`，而不是使程序崩溃。这就是为什么 `.get()` 是从 `HashMap` 中获取一个值的比较安全的方法。

```rust
use std::collections::HashMap;

fn main() {
    let canadian_cities = vec!["Calgary", "Vancouver", "Gimli"];
    let german_cities = vec!["Karlsruhe", "Bad Doberan", "Bielefeld"];

    let mut city_hashmap = HashMap::new();

    for city in canadian_cities {
        city_hashmap.insert(city, "Canada");
    }
    for city in german_cities {
        city_hashmap.insert(city, "Germany");
    }

    println!("{:?}", city_hashmap["Bielefeld"]);
    println!("{:?}", city_hashmap.get("Bielefeld"));
    println!("{:?}", city_hashmap.get("Bielefeldd"));
}
```

这个打印:

```text
"Germany"
Some("Germany")
None
```

这是因为*Bielefeld*存在，但*Bielefeldd*不存在。

如果`HashMap`已经有一个键，当你试图把它放进去时，它将覆盖它的值。

```rust
use std::collections::HashMap;

fn main() {
    let mut book_hashmap = HashMap::new();

    book_hashmap.insert(1, "L'Allemagne Moderne");
    book_hashmap.insert(1, "Le Petit Prince");
    book_hashmap.insert(1, "섀도우 오브 유어 스마일");
    book_hashmap.insert(1, "Eye of the World");

    println!("{:?}", book_hashmap.get(&1));
}
```

这将打印出 `Some("Eye of the World")`，因为它是你最后使用 `.insert()` 的条目。

检查一个条目是否存在是很容易的，因为你可以用 `.get()` 检查，它给出了 `Option`。

```rust
use std::collections::HashMap;

fn main() {
    let mut book_hashmap = HashMap::new();

    book_hashmap.insert(1, "L'Allemagne Moderne");

    if book_hashmap.get(&1).is_none() { // is_none() returns a bool: true if it's None, false if it's Some
        book_hashmap.insert(1, "Le Petit Prince");
    }

    println!("{:?}", book_hashmap.get(&1));
}
```

这个打印`Some("L\'Allemagne Moderne")`是因为已经有了key为`1`的，所以我们没有插入`Le Petit Prince`。

`HashMap`有一个非常有趣的方法，叫做`.entry()`，你一定要试试。有了它，你可以在没有键的情况下，用如`.or_insert()`这类方法来插入值。有趣的是，它还给出了一个可变引用，所以如果你想的话，你可以改变它。首先是一个例子，我们只是在每次插入书名到`HashMap`时插入一个`true`。

让我们假设我们有一个图书馆，并希望跟踪我们的书籍。

```rust
use std::collections::HashMap;

fn main() {
    let book_collection = vec!["L'Allemagne Moderne", "Le Petit Prince", "Eye of the World", "Eye of the World"]; // Eye of the World appears twice

    let mut book_hashmap = HashMap::new();

    for book in book_collection {
        book_hashmap.entry(book).or_insert(true);
    }
    for (book, true_or_false) in book_hashmap {
        println!("Do we have {}? {}", book, true_or_false);
    }
}
```

这个将打印:

```text
Do we have Eye of the World? true
Do we have Le Petit Prince? true
Do we have L'Allemagne Moderne? true
```

但这并不是我们想要的。也许最好是数一下书的数量，这样我们就知道*世界之眼* 有两本。首先让我们看看`.entry()`做了什么，以及`.or_insert()`做了什么。`.entry()`其实是返回了一个名为`Entry`的`enum`。

```rust
pub fn entry(&mut self, key: K) -> Entry<K, V> // 🚧
```


[Entry文档页](https://doc.rust-lang.org/std/collections/hash_map/enum.Entry.html)。下面是其代码的简单版本。`K`表示key，`V`表示value。

```rust
// 🚧
use std::collections::hash_map::*;

enum Entry<K, V> {
    Occupied(OccupiedEntry<K, V>),
    Vacant(VacantEntry<K, V>),
}
```

然后当我们调用`.or_insert()`时，它就会查看枚举，并决定该怎么做。

```rust
fn or_insert(self, default: V) -> &mut V { // 🚧
    match self {
        Occupied(entry) => entry.into_mut(),
        Vacant(entry) => entry.insert(default),
    }
}
```

有趣的是，它返回一个`mut`的引用。`&mut V`. 这意味着你可以使用`let`将其附加到一个变量上，并改变变量来改变`HashMap`中的值。所以对于每本书，如果没有条目，我们就会插入一个0。而如果有的话，我们将在引用上使用`+= 1`来增加数字。现在它看起来像这样:

```rust
use std::collections::HashMap;

fn main() {
    let book_collection = vec!["L'Allemagne Moderne", "Le Petit Prince", "Eye of the World", "Eye of the World"];

    let mut book_hashmap = HashMap::new();

    for book in book_collection {
        let return_value = book_hashmap.entry(book).or_insert(0); // return_value is a mutable reference. If nothing is there, it will be 0
        *return_value +=1; // Now return_value is at least 1. And if there was another book, it will go up by 1
    }

    for (book, number) in book_hashmap {
        println!("{}, {}", book, number);
    }
}
```


重要的部分是`let return_value = book_hashmap.entry(book).or_insert(0);`。如果去掉 `let`，你会得到 `book_hashmap.entry(book).or_insert(0)`。如果没有`let`，它什么也不做:它插入了0，没有获取指向0的可变引用。所以我们把它绑定到`return_value`上，这样我们就可以保留0。然后我们把值增加1，这样`HashMap`中的每本书都至少有1。然后当`.entry()`再看*世界之眼*时，它不会插入任何东西，但它给我们一个可变的1。然后我们把它增加到2，所以它才会打印出这样的结果。

```text
L'Allemagne Moderne, 1
Le Petit Prince, 1
Eye of the World, 2
```


你也可以用`.or_insert()`做一些事情，比如插入一个vec，然后推入数据。让我们假设我们问街上的男人和女人他们对一个政治家的看法。他们给出的评分从0到10。然后我们要把这些数字放在一起，看看这个政治家是更受男人欢迎还是女人欢迎。它可以是这样的。


```rust
use std::collections::HashMap;

fn main() {
    let data = vec![ // This is the raw data
        ("male", 9),
        ("female", 5),
        ("male", 0),
        ("female", 6),
        ("female", 5),
        ("male", 10),
    ];

    let mut survey_hash = HashMap::new();

    for item in data { // This gives a tuple of (&str, i32)
        survey_hash.entry(item.0).or_insert(Vec::new()).push(item.1); // This pushes the number into the Vec inside
    }

    for (male_or_female, numbers) in survey_hash {
        println!("{:?}: {:?}", male_or_female, numbers);
    }
}
```

这个打印:

```text
"female", [5, 6, 5]
"male", [9, 0, 10]
```

重要的一行是:`survey_hash.entry(item.0).or_insert(Vec::new()).push(item.1);`，所以如果它看到 "女"，就会检查`HashMap`中是否已经有 "女"。如果没有，它就会插入一个`Vec::new()`，然后把数字推入。如果它看到 "女性"已经在`HashMap`中，它将不会插入一个新的Vec，而只是将数字推入其中。

### HashSet和BTreeSet

`HashSet`实际上是一个只有key的`HashMap`。在[HashSet的页面](https://doc.rust-lang.org/std/collections/struct.HashSet.html)上面有解释。


`A hash set implemented as a HashMap where the value is ().` 所以这是一个`HashMap`，有键，没有值。

如果你只是想知道一个键是否存在，或者不存在，你经常会使用`HashSet`。

想象一下，你有100个随机数，每个数字在1和100之间。如果你这样做，有些数字会出现不止一次，而有些数字根本不会出现。如果你把它们放到`HashSet`中，那么你就会有一个所有出现的数字的列表。

```rust
use std::collections::HashSet;

fn main() {
    let many_numbers = vec![
        94, 42, 59, 64, 32, 22, 38, 5, 59, 49, 15, 89, 74, 29, 14, 68, 82, 80, 56, 41, 36, 81, 66,
        51, 58, 34, 59, 44, 19, 93, 28, 33, 18, 46, 61, 76, 14, 87, 84, 73, 71, 29, 94, 10, 35, 20,
        35, 80, 8, 43, 79, 25, 60, 26, 11, 37, 94, 32, 90, 51, 11, 28, 76, 16, 63, 95, 13, 60, 59,
        96, 95, 55, 92, 28, 3, 17, 91, 36, 20, 24, 0, 86, 82, 58, 93, 68, 54, 80, 56, 22, 67, 82,
        58, 64, 80, 16, 61, 57, 14, 11];

    let mut number_hashset = HashSet::new();

    for number in many_numbers {
        number_hashset.insert(number);
    }

    let hashset_length = number_hashset.len(); // The length tells us how many numbers are in it
    println!("There are {} unique numbers, so we are missing {}.", hashset_length, 100 - hashset_length);

    // Let's see what numbers we are missing
    let mut missing_vec = vec![];
    for number in 0..100 {
        if number_hashset.get(&number).is_none() { // If .get() returns None,
            missing_vec.push(number);
        }
    }

    print!("It does not contain: ");
    for number in missing_vec {
        print!("{} ", number);
    }
}
```

这个打印:

```text
There are 66 unique numbers, so we are missing 34.
It does not contain: 1 2 4 6 7 9 12 21 23 27 30 31 39 40 45 47 48 50 52 53 62 65 69 70 72 75 77 78 83 85 88 97 98 99
```

`BTreeSet`与`HashSet`相似，就像`BTreeMap`与`HashMap`相似一样。如果我们把`HashSet`中的每一项都打印出来，就不知道顺序是什么了。

```rust
for entry in number_hashset { // 🚧
    print!("{} ", entry);
}
```

也许它能打印出这个。`67 28 42 25 95 59 87 11 5 81 64 34 8 15 13 86 10 89 63 93 49 41 46 57 60 29 17 22 74 43 32 38 36 76 71 18 14 84 61 16 35 90 56 54 91 19 94 44 3 0 68 80 51 92 24 20 82 26 58 33 55 96 37 66 79 73`. 但它几乎不会再以同样的方式打印。

在这里也一样，如果你决定需要订购的话，很容易把你的`HashSet`改成`BTreeSet`。在我们的代码中，我们只需要做两处改动，就可以从`HashSet`切换到`BTreeSet`。

```rust
use std::collections::BTreeSet; // Change HashSet to BTreeSet

fn main() {
    let many_numbers = vec![
        94, 42, 59, 64, 32, 22, 38, 5, 59, 49, 15, 89, 74, 29, 14, 68, 82, 80, 56, 41, 36, 81, 66,
        51, 58, 34, 59, 44, 19, 93, 28, 33, 18, 46, 61, 76, 14, 87, 84, 73, 71, 29, 94, 10, 35, 20,
        35, 80, 8, 43, 79, 25, 60, 26, 11, 37, 94, 32, 90, 51, 11, 28, 76, 16, 63, 95, 13, 60, 59,
        96, 95, 55, 92, 28, 3, 17, 91, 36, 20, 24, 0, 86, 82, 58, 93, 68, 54, 80, 56, 22, 67, 82,
        58, 64, 80, 16, 61, 57, 14, 11];

    let mut number_btreeset = BTreeSet::new(); // Change HashSet to BTreeSet

    for number in many_numbers {
        number_btreeset.insert(number);
    }
    for entry in number_btreeset {
        print!("{} ", entry);
    }
}
```

现在会按顺序打印。`0 3 5 8 10 11 13 14 15 16 17 18 19 20 22 24 25 26 28 29 32 33 34 35 36 37 38 41 42 43 44 46 49 51 54 55 56 57 58 59 60 61 63 64 66 67 68 71 73 74 76 79 80 81 82 84 86 87 89 90 91 92 93 94 95 96`.

### 二叉堆

`BinaryHeap`是一种有趣的集合类型，因为它大部分是无序的，但也有一点秩序。它把最大的元素放在前面，但其他元素是按任何顺序排列的。

我们将用另一个元素列表来举例，但这次数据少些。

```rust
use std::collections::BinaryHeap;

fn show_remainder(input: &BinaryHeap<i32>) -> Vec<i32> { // This function shows the remainder in the BinaryHeap. Actually an iterator would be
                                                         // faster than a function - we will learn them later.
    let mut remainder_vec = vec![];
    for number in input {
        remainder_vec.push(*number)
    }
    remainder_vec
}

fn main() {
    let many_numbers = vec![0, 5, 10, 15, 20, 25, 30]; // These numbers are in order

    let mut my_heap = BinaryHeap::new();

    for number in many_numbers {
        my_heap.push(number);
    }

    while let Some(number) = my_heap.pop() { // .pop() returns Some(number) if a number is there, None if not. It pops from the front
        println!("Popped off {}. Remaining numbers are: {:?}", number, show_remainder(&my_heap));
    }
}
```

这个打印:

```text
Popped off 30. Remaining numbers are: [25, 15, 20, 0, 10, 5]
Popped off 25. Remaining numbers are: [20, 15, 5, 0, 10]
Popped off 20. Remaining numbers are: [15, 10, 5, 0]
Popped off 15. Remaining numbers are: [10, 0, 5]
Popped off 10. Remaining numbers are: [5, 0]
Popped off 5. Remaining numbers are: [0]
Popped off 0. Remaining numbers are: []
```

你可以看到，0指数的数字总是最大的。25, 20, 15, 10, 5, 然后是0.

使用`BinaryHeap<(u8, &str)>`的一个好方法是用于一个事情的集合。这里我们创建一个`BinaryHeap<(u8, &str)>`，其中`u8`是任务重要性的数字。`&str`是对要做的事情的描述。

```rust
use std::collections::BinaryHeap;

fn main() {
    let mut jobs = BinaryHeap::new();

    // Add jobs to do throughout the day
    jobs.push((100, "Write back to email from the CEO"));
    jobs.push((80, "Finish the report today"));
    jobs.push((5, "Watch some YouTube"));
    jobs.push((70, "Tell your team members thanks for always working hard"));
    jobs.push((30, "Plan who to hire next for the team"));

    while let Some(job) = jobs.pop() {
        println!("You need to: {}", job.1);
    }
}
```

这将一直打印:

```text
You need to: Write back to email from the CEO
You need to: Finish the report today
You need to: Tell your team members thanks for always working hard
You need to: Plan who to hire next for the team
You need to: Watch some YouTube
```

### VecDeque

`VecDeque`就是一个`Vec`，既能从前面弹出item，又能从后面弹出item。Rust有`VecDeque`是因为`Vec`很适合从后面(最后一个元素)弹出，但从前面弹出就不那么好了。当你在`Vec`上使用`.pop()`的时候，它只是把右边最后一个item取下来，其他的都不会动。但是如果你把它从其他部分取下来，右边的所有元素都会向左移动一个位置。你可以在`.remove()`的描述中看到这一点。


```text
Removes and returns the element at position index within the vector, shifting all elements after it to the left.
```

所以如果你这样做:

```rust
fn main() {
    let mut my_vec = vec![9, 8, 7, 6, 5];
    my_vec.remove(0);
}
```

它将删除 `9`。索引1中的`8`将移到索引0，索引2中的`7`将移到索引1，以此类推。想象一下，一个大停车场，每当有一辆车离开时，右边所有的车都要移过来。

比如说，这对计算机来说是一个*很大*的工作量。事实上，如果你在playground上运行它，它可能会因为工作太多而直接放弃。

```rust
fn main() {
    let mut my_vec = vec![0; 600_000];
    for i in 0..600000 {
        my_vec.remove(0);
    }
}
```

这是60万个零的`Vec`。每次你用`remove(0)`，它就会把每个零向左移动一个空格。然后它就会做60万次。

用`VecDeque`就不用担心这个问题了。它通常比`Vec`慢一点，但如果你要在两端都做事情，那么它就快多了。你可以直接用`VecDeque::from`与`Vec`来创建一个。那么我们上面的代码就是这样的。

```rust
use std::collections::VecDeque;

fn main() {
    let mut my_vec = VecDeque::from(vec![0; 600000]);
    for i in 0..600000 {
        my_vec.pop_front(); // pop_front is like .pop but for the front
    }
}
```

现在速度快了很多，在playground上，它在一秒内完成，而不是放弃。

在接下来的这个例子中，我们在一个`Vec`上做一些事。我们创建一个`VecDeque`，用`.push_front()`把它们放在前面，所以我们添加的第一个元素会在右边。但是我们推送的每一个元素都是一个`(&str, bool)`:`&str`是描述, `false`表示还没有完成。我们用`done()`函数从后面弹出一个元素，但是我们不想删除它。相反，我们把`false`改成`true`，然后把它推到前面，这样我们就可以保留它。

它看起来是这样的:

```rust
use std::collections::VecDeque;

fn check_remaining(input: &VecDeque<(&str, bool)>) { // Each item is a (&str, bool)
    for item in input {
        if item.1 == false {
            println!("You must: {}", item.0);
        }
    }
}

fn done(input: &mut VecDeque<(&str, bool)>) {
    let mut task_done = input.pop_back().unwrap(); // pop off the back
    task_done.1 = true;                            // now it's done - mark as true
    input.push_front(task_done);                   // put it at the front now
}

fn main() {
    let mut my_vecdeque = VecDeque::new();
    let things_to_do = vec!["send email to customer", "add new product to list", "phone Loki back"];

    for thing in things_to_do {
        my_vecdeque.push_front((thing, false));
    }

    done(&mut my_vecdeque);
    done(&mut my_vecdeque);

    check_remaining(&my_vecdeque);

    for task in my_vecdeque {
        print!("{:?} ", task);
    }
}
```

这个打印:

```text
You must: phone Loki back
("add new product to list", true) ("send email to customer", true) ("phone Loki back", false)
```

## ?操作符

有一种更短的方法来处理`Result`(和`Option`)，它比`match`和`if let`更短。它叫做 "问号运算符"，就是`?`。在返回结果的函数后，可以加上`?`。这样就会:

- 如果是`Ok`，返回`Result`里面的内容。
- 如果是`Err`，则将错误传回。

换句话说，它几乎为你做了所有的事情。

我们可以用 `.parse()` 再试一次。我们将编写一个名为 `parse_str` 的函数，试图将 `&str` 变成 `i32`。它看起来像这样:

```rust
use std::num::ParseIntError;

fn parse_str(input: &str) -> Result<i32, ParseIntError> {
    let parsed_number = input.parse::<i32>()?; // Here is the question mark
    Ok(parsed_number)
}

fn main() {}
```

这个函数接收一个 `&str`。如果是 `Ok`，则给出一个 `i32`，包裹在 `Ok` 中。如果是 `Err`，则返回 `ParseIntError`。然后我们尝试解析这个数字，并加上`?`。也就是 "检查是否错误，如果没问题就给出Result里面的内容"。如果有问题，就会返回错误并结束。但如果没问题，就会进入下一行。下一行是`Ok()`里面的数字。我们需要用`Ok`来包装，因为返回的是`Result<i32, ParseIntError>`，而不是`i32`。

现在，我们可以试试我们的函数。让我们看看它对`&str`的vec有什么作用。


```rust
fn parse_str(input: &str) -> Result<i32, std::num::ParseIntError> {
    let parsed_number = input.parse::<i32>()?;
    Ok(parsed_number)
}

fn main() {
    let str_vec = vec!["Seven", "8", "9.0", "nice", "6060"];
    for item in str_vec {
        let parsed = parse_str(item);
        println!("{:?}", parsed);
    }
}
```

这个打印:

```text
Err(ParseIntError { kind: InvalidDigit })
Ok(8)
Err(ParseIntError { kind: InvalidDigit })
Err(ParseIntError { kind: InvalidDigit })
Ok(6060)
```

我们是怎么找到`std::num::ParseIntError`的呢？一个简单的方法就是再 "问"一下编译器。

```rust
fn main() {
    let failure = "Not a number".parse::<i32>();
    failure.rbrbrb(); // ⚠️ Compiler: "What is rbrbrb()???"
}
```

编译器不懂，说。

```text
error[E0599]: no method named `rbrbrb` found for enum `std::result::Result<i32, std::num::ParseIntError>` in the current scope
 --> src\main.rs:3:13
  |
3 |     failure.rbrbrb();
  |             ^^^^^^ method not found in `std::result::Result<i32, std::num::ParseIntError>`
```

所以`std::result::Result<i32, std::num::ParseIntError>`就是我们需要的签名。

我们不需要写 `std::result::Result`，因为 `Result` 总是 "在范围内"(在范围内 = 准备好使用)。Rust对我们经常使用的所有类型都是这样做的，所以我们不必写`std::result::Result`、`std::collections::Vec`等。

我们现在还没有处理文件这样的东西，所以?操作符看起来还不是太有用。但这里有一个无用但快速的例子，说明你如何在单行上使用它。与其用 `.parse()` 创建一个 `i32`，不如做更多。我们将创建一个 `u16`，然后把它变成 `String`，再变成 `u32`，然后再变成 `String`，最后变成 `i32`。

```rust
use std::num::ParseIntError;

fn parse_str(input: &str) -> Result<i32, ParseIntError> {
    let parsed_number = input.parse::<u16>()?.to_string().parse::<u32>()?.to_string().parse::<i32>()?; // Add a ? each time to check and pass it on
    Ok(parsed_number)
}

fn main() {
    let str_vec = vec!["Seven", "8", "9.0", "nice", "6060"];
    for item in str_vec {
        let parsed = parse_str(item);
        println!("{:?}", parsed);
    }
}
```

这打印出同样的东西，但这次我们在一行中处理了三个`Result`。稍后我们将对文件进行处理，因为它们总是返回`Result`，因为很多事情都可能出错。

想象一下:你想打开一个文件，向它写入，然后关闭它。首先你需要成功找到这个文件(这就是一个`Result`)。然后你需要成功地写入它(那是一个`Result`)。对于`?`，你可以在一行上完成。

### When panic and unwrap are good

Rust有一个`panic!`的宏，你可以用它来让程序崩溃。它使用起来很方便。

```rust
fn main() {
    panic!("Time to panic!");
}
```

运行程序时，会显示信息`"Time to panic!"`。`thread 'main' panicked at 'Time to panic!', src\main.rs:2:3`

你会记得`src\main.rs`是目录和文件名，`2:3`是行名和列名。有了这些信息，你就可以找到代码并修复它。

`panic!`是一个很好用的宏，以确保你知道什么时候有变化。例如，这个叫做`prints_three_things`的函数总是从一个向量中打印出索引[0]、[1]和[2]。这没关系，因为我们总是给它一个有三个元素的向量。

```rust
fn prints_three_things(vector: Vec<i32>) {
    println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
    let my_vec = vec![8, 9, 10];
    prints_three_things(my_vec);
}
```

它打印出`8, 9, 10`，一切正常。

但试想一下，后来我们写的代码越来越多，忘记了`my_vec`只能有三个元素。现在`my_vec`在这部分有六个元素。

```rust
fn prints_three_things(vector: Vec<i32>) {
  println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
  let my_vec = vec![8, 9, 10, 10, 55, 99]; // Now my_vec has six things
  prints_three_things(my_vec);
}
```

不会发生错误，因为[0]和[1]和[2]都在这个较长的`Vec`里面。但如果只能有三个元素呢？我们就不会知道有问题了，因为程序不会崩溃。我们应该这样做:

```rust
fn prints_three_things(vector: Vec<i32>) {
    if vector.len() != 3 {
        panic!("my_vec must always have three items") // will panic if the length is not 3
    }
    println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
    let my_vec = vec![8, 9, 10];
    prints_three_things(my_vec);
}
```

现在我们知道，如果向量有6个元素，它应该要崩溃:

```rust
    // ⚠️
fn prints_three_things(vector: Vec<i32>) {
    if vector.len() != 3 {
        panic!("my_vec must always have three items")
    }
    println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
    let my_vec = vec![8, 9, 10, 10, 55, 99];
    prints_three_things(my_vec);
}
```

这样我们就得到了`thread 'main' panicked at 'my_vec must always have three items', src\main.rs:8:9`。多亏了`panic!`，我们现在记得`my_vec`应该只有三个元素。所以`panic!`是一个很好的宏，可以在你的代码中创建提醒。

还有三个与`panic!`类似的宏，你在测试中经常使用。它们分别是 `assert!`, `assert_eq!`, 和 `assert_ne!`.

下面是它们的意思。

- `assert!()`: 如果`()`里面的部分不是真的, 程序就会崩溃.
- `assert_eq!()`:`()`里面的两个元素必须相等。
- `assert_ne!()`:`()`里面的两个元素必须不相等。(*ne*表示不相等)

一些例子。

```rust
fn main() {
    let my_name = "Loki Laufeyson";

    assert!(my_name == "Loki Laufeyson");
    assert_eq!(my_name, "Loki Laufeyson");
    assert_ne!(my_name, "Mithridates");
}
```

这不会有任何作用，因为三个断言宏都没有问题。(这就是我们想要的)

如果你愿意，还可以加个提示信息。

```rust
fn main() {
    let my_name = "Loki Laufeyson";

    assert!(
        my_name == "Loki Laufeyson",
        "{} should be Loki Laufeyson",
        my_name
    );
    assert_eq!(
        my_name, "Loki Laufeyson",
        "{} and Loki Laufeyson should be equal",
        my_name
    );
    assert_ne!(
        my_name, "Mithridates",
        "You entered {}. Input must not equal Mithridates",
        my_name
    );
}
```

这些信息只有在程序崩溃时才会显示。所以如果你运行这个。

```rust
fn main() {
    let my_name = "Mithridates";

    assert_ne!(
        my_name, "Mithridates",
        "You enter {}. Input must not equal Mithridates",
        my_name
    );
}
```

它将显示:

```text
thread 'main' panicked at 'assertion failed: `(left != right)`
  left: `"Mithridates"`,
 right: `"Mithridates"`: You entered Mithridates. Input must not equal Mithridates', src\main.rs:4:5
```

所以它说 "你说左!=右，但左==右"。而且它显示我们的信息说`You entered Mithridates. Input must not equal Mithridates`。

当你在写程序的时候，想让它在出现问题的时候崩溃，`unwrap`是个好注意。当你的代码写完后，把`unwrap`改成其他不会崩溃的东西就好了。

你也可以用`expect`，它和`unwrap`一样，但是更好一些，因为它支持用户自定义信息。教科书通常会给出这样的建议:"如果你经常使用`.unwrap()`, 至少也要用`.expect()`来获得更好的错误信息."

这样会崩溃的:

```rust
   // ⚠️
fn get_fourth(input: &Vec<i32>) -> i32 {
    let fourth = input.get(3).unwrap();
    *fourth
}

fn main() {
    let my_vec = vec![9, 0, 10];
    let fourth = get_fourth(&my_vec);
}
```

错误信息是`thread 'main' panicked at 'called Option::unwrap() on a None value', src\main.rs:7:18`。

现在我们用`expect`来写自己的信息。

```rust
   // ⚠️
fn get_fourth(input: &Vec<i32>) -> i32 {
    let fourth = input.get(3).expect("Input vector needs at least 4 items");
    *fourth
}

fn main() {
    let my_vec = vec![9, 0, 10];
    let fourth = get_fourth(&my_vec);
}
```

又崩溃了，但错误比较多。`thread 'main' panicked at 'Input vector needs at least 4 items', src\main.rs:7:18`. `.expect()`因为这个原因比`.unwrap()`要好一点，但是在`None`上还是会崩溃。现在这里有一个错误的案例，一个函数试图unwrap两次。它需要一个`Vec<Option<i32>>`，所以可能每个部分都会有一个`Some<i32>`，也可能是一个`None`。

```rust
fn try_two_unwraps(input: Vec<Option<i32>>) {
    println!("Index 0 is: {}", input[0].unwrap());
    println!("Index 1 is: {}", input[1].unwrap());
}

fn main() {
    let vector = vec![None, Some(1000)]; // This vector has a None, so it will panic
    try_two_unwraps(vector);
}
```

消息是:``thread 'main' panicked at 'called `Option::unwrap()` on a `None` value', src\main.rs:2:32``。我们不检查行号，就不知道是第一个`.unwrap()`还是第二个`.unwrap()`。最好是检查一下长度，也不要unwrap。不过有了`.expect()`至少会好*一点*。下面是`.expect()`的情况：

```rust
fn try_two_unwraps(input: Vec<Option<i32>>) {
    println!("Index 0 is: {}", input[0].expect("The first unwrap had a None!"));
    println!("Index 1 is: {}", input[1].expect("The second unwrap had a None!"));
}

fn main() {
    let vector = vec![None, Some(1000)];
    try_two_unwraps(vector);
}
```

所以，这是好一点的。`thread 'main' panicked at 'The first unwrap had a None!', src\main.rs:2:32`. 我们也有行号，所以我们可以找到它。


如果你想一直有一个你想选择的值，也可以用`unwrap_or`。如果你这样做，它永远不会崩溃。就是这样的。


- 1)好，因为你的程序不会崩溃，但
- 2)如果你想让程序在出现问题时崩溃，也许不好。

但通常我们都不希望自己的程序崩溃，所以`unwrap_or`是个不错的方法。

```rust
fn main() {
    let my_vec = vec![8, 9, 10];

    let fourth = my_vec.get(3).unwrap_or(&0); // If .get doesn't work, we will make the value &0.
                                              // .get returns a reference, so we need &0 and not 0
                                              // You can write "let *fourth" with a * if you want fourth to be
                                              // a 0 and not a &0, but here we just print so it doesn't matter

    println!("{}", fourth);
}
```

这将打印出 `0`，因为 `.unwrap_or(&0)` 给出了一个 0，即使它是 `None`。

## 特性

我们以前见过trait:`Debug`、`Copy`、`Clone`都是trait。要给一个类型一个trait，就必须实现它。因为`Debug`和其他的trait都很常见，所以我们有自动实现的属性。这就是当你写下`#[derive(Debug)]`所发生的事情:你自动实现了`Debug`。

```rust
#[derive(Debug)]
struct MyStruct {
    number: usize,
}

fn main() {}
```

但是其他的特性就比较困难了，所以需要用`impl`手动实现。例如，`Add`(在`std::ops::Add`处找到)是用来累加两个东西的。但是Rust并不知道你到底要怎么累加，所以你必须告诉它。

```rust
struct ThingsToAdd {
    first_thing: u32,
    second_thing: f32,
}

fn main() {}
```

我们可以累加`first_thing`和`second_thing`，但我们需要提供更多信息。也许我们想要一个`f32`，所以像这样:

```rust
// 🚧
let result = self.second_thing + self.first_thing as f32
```

但也许我们想要一个整数，所以像这样:

```rust
// 🚧
let result = self.second_thing as u32 + self.first_thing
```

或者我们想把`self.first_thing`放在`self.second_thing`旁边，这样加。所以如果我们把55加到33.4，我们要看到的是5533.4，而不是88.4。

所以首先我们看一下如何创建一个trait。关于`trait`，要记住的重要一点是，它们是关于行为的。要创建一个trait，写下单词`trait`，然后创建一些函数。

```rust
struct Animal { // A simple struct - an Animal only has a name
    name: String,
}

trait Dog { // The dog trait gives some functionality
    fn bark(&self) { // It can bark
        println!("Woof woof!");
    }
    fn run(&self) { // and it can run
        println!("The dog is running!");
    }
}

impl Dog for Animal {} // Now Animal has the trait Dog

fn main() {
    let rover = Animal {
        name: "Rover".to_string(),
    };

    rover.bark(); // Now Animal can use bark()
    rover.run();  // and it can use run()
}
```

这个是可以的，但是我们不想打印 "狗在跑"。如果你想的话，你可以改变`trait`给你的方法，但你必须有相同的签名。这意味着它需要接受同样的东西，并返回同样的东西。例如，我们可以改变 `.run()` 的方法，但我们必须遵循签名。签名说

```rust
// 🚧
fn run(&self) {
    println!("The dog is running!");
}
```

`fn run(&self)`的意思是 "fn `run()`以`&self`为参数，不返回任何内容"。所以你不能这样做:

```rust
fn run(&self) -> i32 { // ⚠️
    5
}
```

Rust会说。

```text
   = note: expected fn pointer `fn(&Animal)`
              found fn pointer `fn(&Animal) -> i32`
```

但我们可以做到这一点。

```rust
struct Animal { // A simple struct - an Animal only has a name
    name: String,
}

trait Dog { // The dog trait gives some functionality
    fn bark(&self) { // It can bark
        println!("Woof woof!");
    }
    fn run(&self) { // and it can run
        println!("The dog is running!");
    }
}

impl Dog for Animal {
    fn run(&self) {
        println!("{} is running!", self.name);
    }
}

fn main() {
    let rover = Animal {
        name: "Rover".to_string(),
    };

    rover.bark(); // Now Animal can use bark()
    rover.run();  // and it can use run()
}
```

现在它打印的是 `Rover is running!`。这是好的，因为我们返回的是 `()`，或者说什么都没有，这就是trait所说的。


当你写一个trait的时候，你可以直接写函数签名，但如果你这样做，用户将不得不写函数实现。我们来试试。现在我们把`bark()`和`run()`改成只说`fn bark(&self);`和`fn run(&self);`。这不是一个完整的函数实现，所以必须由用户来写。

```rust
struct Animal {
    name: String,
}

trait Dog {
    fn bark(&self); // bark() says it needs a &self and returns nothing
    fn run(&self); // run() says it needs a &self and returns nothing.
                   // So now we have to write them ourselves.
}

impl Dog for Animal {
    fn bark(&self) {
        println!("{}, stop barking!!", self.name);
    }
    fn run(&self) {
        println!("{} is running!", self.name);
    }
}

fn main() {
    let rover = Animal {
        name: "Rover".to_string(),
    };

    rover.bark();
    rover.run();
}
```

所以，当你创建一个trait时，你必须思考:"我应该写哪些功能？而用户应该写哪些函数？" 如果你认为用户每次使用函数的方式应该是一样的，那么就把函数写出来。如果你认为用户会以不同的方式使用，那就写出函数签名即可。

所以，让我们尝试为我们的struct实现Display特性。首先我们将创建一个简单的结构体:

```rust
struct Cat {
    name: String,
    age: u8,
}

fn main() {
    let mr_mantle = Cat {
        name: "Reggie Mantle".to_string(),
        age: 4,
    };
}
```

现在我们要打印`mr_mantle`。调试很容易得出。

```rust
#[derive(Debug)]
struct Cat {
    name: String,
    age: u8,
}

fn main() {
    let mr_mantle = Cat {
        name: "Reggie Mantle".to_string(),
        age: 4,
    };

    println!("Mr. Mantle is a {:?}", mr_mantle);
}
```

但Debug打印不是最漂亮的方式，因为它看起来是这样的:

```text
Mr. Mantle is a Cat { name: "Reggie Mantle", age: 4 }
```

因此，如果我们想要更好的打印，就需要实现`Display`为`Cat`。在[https://doc.rust-lang.org/std/fmt/trait.Display.html](https://doc.rust-lang.org/std/fmt/trait.Display.html)上我们可以看到Display的信息，还有一个例子。它说

```rust
use std::fmt;

struct Position {
    longitude: f32,
    latitude: f32,
}

impl fmt::Display for Position {
    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
        write!(f, "({}, {})", self.longitude, self.latitude)
    }
}

fn main() {}
```

有些部分我们还不明白，比如`<'_>`和`f`在做什么。但我们理解`Position`结构体:它只是两个`f32`。我们也明白，`self.longitude`和`self.latitude`是结构体中的字段。所以，也许我们的结构体就可以用这个代码，用`self.name`和`self.age`。另外，`write!`看起来很像`println!`，所以很熟悉。所以我们这样写。

```rust
use std::fmt;

struct Cat {
    name: String,
    age: u8,
}

impl fmt::Display for Cat {
    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
        write!(f, "{} is a cat who is {} years old.", self.name, self.age)
    }
}

fn main() {}
```

让我们添加一个`fn main()`。现在我们的代码是这样的。

```rust
use std::fmt;

struct Cat {
    name: String,
    age: u8,
}

impl fmt::Display for Cat {
  fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
      write!(f, "{} is a cat who is {} years old.", self.name, self.age)
  }
}

fn main() {
    let mr_mantle = Cat {
        name: "Reggie Mantle".to_string(),
        age: 4,
    };

    println!("{}", mr_mantle);
}
```

成功了! 现在，当我们使用`{}`打印时，我们得到`Reggie Mantle is a cat who is 4 years old.`。这看起来好多了。


顺便说一下，如果你实现了`Display`，那么你就可以免费得到`ToString`的特性。这是因为你使用`format!`宏来实现`.fmt()`函数，这让你可以用`.to_string()`来创建一个`String`。所以我们可以做这样的事情，我们把`reggie_mantle`传给一个想要`String`的函数，或者其他任何东西。

```rust
use std::fmt;
struct Cat {
    name: String,
    age: u8,
}

impl fmt::Display for Cat {
    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
        write!(f, "{} is a cat who is {} years old.", self.name, self.age)
    }
}

fn print_cats(pet: String) {
    println!("{}", pet);
}

fn main() {
    let mr_mantle = Cat {
        name: "Reggie Mantle".to_string(),
        age: 4,
    };

    print_cats(mr_mantle.to_string()); // Turn him into a String here
    println!("Mr. Mantle's String is {} letters long.", mr_mantle.to_string().chars().count()); // Turn him into chars and count them
}
```

这个打印:

```text
Reggie Mantle is a cat who is 4 years old.
Mr. Mantle's String is 42 letters long.
```




关于trait，要记住的是，它们是关于某些东西的行为。你的`struct`是如何行动的？它能做什么？这就是trait的作用。如果你想想我们到目前为止所看到的一些trait，它们都是关于行为的:`Copy`是一个类型可以做的事情。`Display`也是一个类型能做的事情。`ToString`是另一个trait，它也是一个类型可以做的事情:它可以变化成一个`String`。在我们的 `Dog` trait中，*Dog*这个词并不意味着你能做的事情，但它给出了一些让它做事情的方法。
 你也可以为 `struct Poodle` 或 `struct Beagle` 实现它，它们都会得到 `Dog` 方法。


让我们再看一个与单纯行为联系更紧密的例子。我们将想象一个有一些简单角色的幻想游戏。一个是`Monster`，另外两个是`Wizard`和`Ranger`。`Monster`只是有`health`，所以我们可以攻击它，其他两个还没有什么。但是我们做了两个trait。一个叫`FightClose`，让你近身作战。另一个是`FightFromDistance`，让你在远处战斗。只有`Ranger`可以使用`FightFromDistance`。下面是它的样子:

```rust
struct Monster {
    health: i32,
}

struct Wizard {}
struct Ranger {}

trait FightClose {
    fn attack_with_sword(&self, opponent: &mut Monster) {
        opponent.health -= 10;
        println!(
            "You attack with your sword. Your opponent now has {} health left.",
            opponent.health
        );
    }
    fn attack_with_hand(&self, opponent: &mut Monster) {
        opponent.health -= 2;
        println!(
            "You attack with your hand. Your opponent now has {} health left.",
            opponent.health
        );
    }
}
impl FightClose for Wizard {}
impl FightClose for Ranger {}

trait FightFromDistance {
    fn attack_with_bow(&self, opponent: &mut Monster, distance: u32) {
        if distance < 10 {
            opponent.health -= 10;
            println!(
                "You attack with your bow. Your opponent now has {} health left.",
                opponent.health
            );
        }
    }
    fn attack_with_rock(&self, opponent: &mut Monster, distance: u32) {
        if distance < 3 {
            opponent.health -= 4;
        }
        println!(
            "You attack with your rock. Your opponent now has {} health left.",
            opponent.health
        );
    }
}
impl FightFromDistance for Ranger {}

fn main() {
    let radagast = Wizard {};
    let aragorn = Ranger {};

    let mut uruk_hai = Monster { health: 40 };

    radagast.attack_with_sword(&mut uruk_hai);
    aragorn.attack_with_bow(&mut uruk_hai, 8);
}
```

这个打印:

```text
You attack with your sword. Your opponent now has 30 health left.
You attack with your bow. Your opponent now has 20 health left.
```

我们在trait里面一直传递`self`，但是我们现在不能用它做什么。那是因为 Rust 不知道什么类型会使用它。它可能是一个 `Wizard`，也可能是一个 `Ranger`，也可能是一个叫做 `Toefocfgetobjtnode` 的新结构，或者其他任何东西。为了让`self`具有一定的功能，我们可以在trait中添加必要的trait。比如说，如果我们想用`{:?}`打印，那么我们就需要`Debug`。你只要把它写在`:`(冒号)后面，就可以把它添加到trait中。现在我们的代码是这样的。


```rust
struct Monster {
    health: i32,
}

#[derive(Debug)] // Now Wizard has Debug
struct Wizard {
    health: i32, // Now Wizard has health
}
#[derive(Debug)] // So does Ranger
struct Ranger {
    health: i32, // So does Ranger
}

trait FightClose: std::fmt::Debug { // Now a type needs Debug to use FightClose
    fn attack_with_sword(&self, opponent: &mut Monster) {
        opponent.health -= 10;
        println!(
            "You attack with your sword. Your opponent now has {} health left. You are now at: {:?}", // We can now print self with {:?} because we have Debug
            opponent.health, &self
        );
    }
    fn attack_with_hand(&self, opponent: &mut Monster) {
        opponent.health -= 2;
        println!(
            "You attack with your hand. Your opponent now has {} health left.  You are now at: {:?}",
            opponent.health, &self
        );
    }
}
impl FightClose for Wizard {}
impl FightClose for Ranger {}

trait FightFromDistance: std::fmt::Debug { // We could also do trait FightFromDistance: FightClose because FightClose needs Debug
    fn attack_with_bow(&self, opponent: &mut Monster, distance: u32) {
        if distance < 10 {
            opponent.health -= 10;
            println!(
                "You attack with your bow. Your opponent now has {} health left.  You are now at: {:?}",
                opponent.health, self
            );
        }
    }
    fn attack_with_rock(&self, opponent: &mut Monster, distance: u32) {
        if distance < 3 {
            opponent.health -= 4;
        }
        println!(
            "You attack with your rock. Your opponent now has {} health left.  You are now at: {:?}",
            opponent.health, self
        );
    }
}
impl FightFromDistance for Ranger {}

fn main() {
    let radagast = Wizard { health: 60 };
    let aragorn = Ranger { health: 80 };

    let mut uruk_hai = Monster { health: 40 };

    radagast.attack_with_sword(&mut uruk_hai);
    aragorn.attack_with_bow(&mut uruk_hai, 8);
}
```

现在这个打印:

```text
You attack with your sword. Your opponent now has 30 health left. You are now at: Wizard { health: 60 }
You attack with your bow. Your opponent now has 20 health left.  You are now at: Ranger { health: 80 }
```

在真实的游戏中，可能最好为每个类型重写这个，因为`You are now at: Wizard { health: 60 }`看起来有点可笑。这也是为什么trait里面的方法通常很简单，因为你不知道什么类型会使用它。例如，你不能写出 `self.0 += 10` 这样的东西。但是这个例子表明，我们可以在我们正在写的trait里面使用其他的trait。当我们这样做的时候，我们会得到一些我们可以使用的方法。



另外一种使用trait的方式是使用所谓的`trait bounds`。意思是 "通过一个trait进行限制"。trait限制很简单，因为一个trait实际上不需要任何方法，或者说根本不需要任何东西。让我们用类似但不同的东西重写我们的代码。这次我们的trait没有任何方法，但我们有其他需要trait使用的函数。

```rust
use std::fmt::Debug;  // So we don't have to write std::fmt::Debug every time now

struct Monster {
    health: i32,
}

#[derive(Debug)]
struct Wizard {
    health: i32,
}
#[derive(Debug)]
struct Ranger {
    health: i32,
}

trait Magic{} // No methods for any of these traits. They are just trait bounds
trait FightClose {}
trait FightFromDistance {}

impl FightClose for Ranger{} // Each type gets FightClose,
impl FightClose for Wizard {}
impl FightFromDistance for Ranger{} // but only Ranger gets FightFromDistance
impl Magic for Wizard{}  // and only Wizard gets Magic

fn attack_with_bow<T: FightFromDistance + Debug>(character: &T, opponent: &mut Monster, distance: u32) {
    if distance < 10 {
        opponent.health -= 10;
        println!(
            "You attack with your bow. Your opponent now has {} health left.  You are now at: {:?}",
            opponent.health, character
        );
    }
}

fn attack_with_sword<T: FightClose + Debug>(character: &T, opponent: &mut Monster) {
    opponent.health -= 10;
    println!(
        "You attack with your sword. Your opponent now has {} health left. You are now at: {:?}",
        opponent.health, character
    );
}

fn fireball<T: Magic + Debug>(character: &T, opponent: &mut Monster, distance: u32) {
    if distance < 15 {
        opponent.health -= 20;
        println!("You raise your hands and cast a fireball! Your opponent now has {} health left. You are now at: {:?}",
    opponent.health, character);
    }
}

fn main() {
    let radagast = Wizard { health: 60 };
    let aragorn = Ranger { health: 80 };

    let mut uruk_hai = Monster { health: 40 };

    attack_with_sword(&radagast, &mut uruk_hai);
    attack_with_bow(&aragorn, &mut uruk_hai, 8);
    fireball(&radagast, &mut uruk_hai, 8);
}
```

这个打印出来的东西几乎是一样的。

```text
You attack with your sword. Your opponent now has 30 health left. You are now at: Wizard { health: 60 }
You attack with your bow. Your opponent now has 20 health left.  You are now at: Ranger { health: 80 }
You raise your hands and cast a fireball! Your opponent now has 0 health left. You are now at: Wizard { health: 60 }
```

所以你可以看到，当你使用traits时，有很多方法可以做同样的事情。这一切都取决于什么对你正在编写的程序最有意义。

现在让我们来看看如何实现一些在Rust中使用的主要trait。

### From trait

*From*是一个非常方便的trait，你知道这一点，因为你已经看到了很多。使用*From*，你可以从一个`&str`创建一个`String`，你也可以用许多其他类型创建多种类型。例如，Vec使用*From*来创建以下类型:

```text
From<&'_ [T]>
From<&'_ mut [T]>
From<&'_ str>
From<&'a Vec<T>>
From<[T; N]>
From<BinaryHeap<T>>
From<Box<[T]>>
From<CString>
From<Cow<'a, [T]>>
From<String>
From<Vec<NonZeroU8>>
From<Vec<T>>
From<VecDeque<T>>
```

这里有很多`Vec::from()`我们还没有用过。我们来做几个，看看会怎么样:

```rust
use std::fmt::Display; // We will make a generic function to print them so we want Display

fn print_vec<T: Display>(input: &Vec<T>) { // Take any Vec<T> if type T has Display
    for item in input {
        print!("{} ", item);
    }
    println!();
}

fn main() {

    let array_vec = Vec::from([8, 9, 10]); // Try from an array
    print_vec(&array_vec);

    let str_vec = Vec::from("What kind of vec will I be?"); // An array from a &str? This will be interesting
    print_vec(&str_vec);

    let string_vec = Vec::from("What kind of vec will a String be?".to_string()); // Also from a String
    print_vec(&string_vec);
}
```

它打印的内容如下。

```text
8 9 10
87 104 97 116 32 107 105 110 100 32 111 102 32 118 101 99 32 119 105 108 108 32 73 32 98 101 63
87 104 97 116 32 107 105 110 100 32 111 102 32 118 101 99 32 119 105 108 108 32 97 32 83 116 114 105 110 103 32 98 101 63
```

如果从类型上看，第二个和第三个向量是`Vec<u8>`，也就是`&str`和`String`的字节。所以你可以看到`From`是非常灵活的，用的也很多。我们用自己的类型来试试。

我们将创建两个结构体，然后为其中一个结构体实现`From`。一个结构体将是`City`，另一个结构体将是`Country`。我们希望能够做到这一点。`let country_name = Country::from(vector_of_cities)`.

它看起来是这样的:

```rust
#[derive(Debug)] // So we can print City
struct City {
    name: String,
    population: u32,
}

impl City {
    fn new(name: &str, population: u32) -> Self { // just a new function
        Self {
            name: name.to_string(),
            population,
        }
    }
}
#[derive(Debug)] // Country also needs to be printed
struct Country {
    cities: Vec<City>, // Our cities go in here
}

impl From<Vec<City>> for Country { // Note: we don't have to write From<City>, we can also do
                                   // From<Vec<City>>. So we can also implement on a type that
                                   // we didn't create
    fn from(cities: Vec<City>) -> Self {
        Self { cities }
    }
}

impl Country {
    fn print_cities(&self) { // function to print the cities in Country
        for city in &self.cities {
            // & because Vec<City> isn't Copy
            println!("{:?} has a population of {:?}.", city.name, city.population);
        }
    }
}

fn main() {
    let helsinki = City::new("Helsinki", 631_695);
    let turku = City::new("Turku", 186_756);

    let finland_cities = vec![helsinki, turku]; // This is the Vec<City>
    let finland = Country::from(finland_cities); // So now we can use From

    finland.print_cities();
}
```

这个将打印:

```text
"Helsinki" has a population of 631695.
"Turku" has a population of 186756.
```

你可以看到，`From`很容易从你没有创建的类型中实现，比如`Vec`、`i32`等等。这里还有一个例子，我们创建一个有两个向量的向量。第一个向量存放偶数，第二个向量存放奇数。对于`From`，你可以给它一个`i32`的向量，它会把它变成`Vec<Vec<i32>>`:一个容纳`i32`的向量。

```rust
use std::convert::From;

struct EvenOddVec(Vec<Vec<i32>>);

impl From<Vec<i32>> for EvenOddVec {
    fn from(input: Vec<i32>) -> Self {
        let mut even_odd_vec: Vec<Vec<i32>> = vec![vec![], vec![]]; // A vec with two empty vecs inside
                                                                    // This is the return value but first we must fill it
        for item in input {
            if item % 2 == 0 {
                even_odd_vec[0].push(item);
            } else {
                even_odd_vec[1].push(item);
            }
        }
        Self(even_odd_vec) // Now it is done so we return it as Self (Self = EvenOddVec)
    }
}

fn main() {
    let bunch_of_numbers = vec![8, 7, -1, 3, 222, 9787, -47, 77, 0, 55, 7, 8];
    let new_vec = EvenOddVec::from(bunch_of_numbers);

    println!("Even numbers: {:?}\nOdd numbers: {:?}", new_vec.0[0], new_vec.0[1]);
}
```

这个打印:

```text
Even numbers: [8, 222, 0, 8]
Odd numbers: [7, -1, 3, 9787, -47, 77, 55, 7]
```

像 `EvenOddVec` 这样的类型可能最好是通用 `T`，这样我们就可以使用许多数字类型。如果你想练习的话，你可以试着把这个例子做成通用的。

### 在函数中使用字符串和&str

有时你想让一个函数可以同时接受 `String` 和 `&str`。你可以通过泛型和 `AsRef` 特性来实现这一点。`AsRef` 用于从一个类型向另一个类型提供引用。如果你看看 `String` 的文档，你可以看到它对许多类型都有 `AsRef`。

[https://doc.rust-lang.org/std/string/struct.String.html](https://doc.rust-lang.org/std/string/struct.String.html)

下面是它们的一些函数签名。

`AsRef<str>`:

```rust
// 🚧
impl AsRef<str> for String

fn as_ref(&self) -> &str
```

`AsRef<[u8]>`:

```rust
// 🚧
impl AsRef<[u8]> for String

fn as_ref(&self) -> &[u8]
```

`AsRef<OsStr>`:

```rust
// 🚧
impl AsRef<OsStr> for String

fn as_ref(&self) -> &OsStr
```

你可以看到，它需要`&self`，并给出另一个类型的引用。这意味着，如果你有一个通用类型T，你可以说它需要`AsRef<str>`。如果你这样做，它将能够使用一个`&str`和一个`String`。

我们先说说泛型函数。这个还不能用。

```rust
fn print_it<T>(input: T) {
    println!("{}", input) // ⚠️
}

fn main() {
    print_it("Please print me");
}
```

Rust说`error[E0277]: T doesn't implement std::fmt::Display`。所以我们会要求T实现Display。

```rust
use std::fmt::Display;

fn print_it<T: Display>(input: T) {
    println!("{}", input)
}

fn main() {
    print_it("Please print me");
}
```

现在可以用了，打印出`Please print me`。这是好的，但T仍然可以是多种类型。
可以是`i8`，也可以是`f32`，或者其他任何实现了`Display`的类型。我们加上`AsRef<str>`，现在T需要`AsRef<str>`和`Display`。

```rust
use std::fmt::Display;

fn print_it<T: AsRef<str> + Display>(input: T) {
    println!("{}", input)
}

fn main() {
    print_it("Please print me");
    print_it("Also, please print me".to_string());
    // print_it(7); <- This will not print
}
```

现在，它不会接受`i8`这样的类型。

不要忘了，当函数变长时，你可以用`where`来写不同的函数。如果我们加上Debug，那么就会变成`fn print_it<T: AsRef<str> + Display + Debug>(input: T)`，这一行就很长了。所以我们可以这样写。

```rust
use std::fmt::{Debug, Display}; // add Debug

fn print_it<T>(input: T) // Now this line is easy to read
where
    T: AsRef<str> + Debug + Display, // and these traits are easy to read
{
    println!("{}", input)
}

fn main() {
    print_it("Please print me");
    print_it("Also, please print me".to_string());
}
```

## 链式方法

Rust是一种系统编程语言，就像C和C++一样，它的代码可以写成独立的命令，单独成行，但它也有函数式风格。两种风格都可以，但函数式通常比较短。下面以非函数式(称为 "命令式")为例，让`Vec`从1到10。

```rust
fn main() {
    let mut new_vec = Vec::new();
    let mut counter = 1;

    while counter < 11 {
        new_vec.push(counter);
        counter += 1;
    }

    println!("{:?}", new_vec);
}
```

这个打印`[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`。

而这里是函数式风格的例子:

```rust
fn main() {
    let new_vec = (1..=10).collect::<Vec<i32>>();
    // Or you can write it like this:
    // let new_vec: Vec<i32> = (1..=10).collect();
    println!("{:?}", new_vec);
}
```

`.collect()`可以为很多类型做集合，所以我们要告诉它类型。

用函数式可以链接方法。"链接方法"的意思是把很多方法放在一个语句中。下面是一个很多方法链在一起的例子。

```rust
fn main() {
    let my_vec = vec![0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    let new_vec = my_vec.into_iter().skip(3).take(4).collect::<Vec<i32>>();

    println!("{:?}", new_vec);
}
```

这样就创建了一个`[3, 4, 5, 6]`的Vec。这一行的信息量很大，所以把每个方法放在新的一行上会有帮助。让我们这样做，以使其更容易阅读。

```rust
fn main() {
    let my_vec = vec![0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    let new_vec = my_vec
        .into_iter() // "iterate" over the items (iterate = work with each item inside it). into_iter() gives us owned values, not references
        .skip(3) // skip over three items: 0, 1, and 2
        .take(4) // take the next four: 3, 4, 5, and 6
        .collect::<Vec<i32>>(); // put them in a new Vec<i32>

    println!("{:?}", new_vec);
}
```

当你了解闭包和迭代器时，你可以最好地使用这种函数式。所以我们接下来将学习它们。

## 迭代器

迭代器是一个构造，它可以给你集合中的元素，一次一个。实际上，我们已经使用了很多迭代器:`for`循环给你一个迭代器。当你想在其他时候使用迭代器时，你必须选择什么样的迭代器:

- `.iter()` 引用的迭代器
- `.iter_mut()` 可变引用的迭代器
- `.into_iter()` 值的迭代器(不是引用)

`for`循环其实只是一个拥有值的迭代器。这就是为什么可以让它变得可变，然后你可以在使用的时候改变值。

我们可以这样使用迭代器。

```rust
fn main() {
    let vector1 = vec![1, 2, 3]; // we will use .iter() and .into_iter() on this one
    let vector1_a = vector1.iter().map(|x| x + 1).collect::<Vec<i32>>();
    let vector1_b = vector1.into_iter().map(|x| x * 10).collect::<Vec<i32>>();

    let mut vector2 = vec![10, 20, 30]; // we will use .iter_mut() on this one
    vector2.iter_mut().for_each(|x| *x +=100);

    println!("{:?}", vector1_a);
    println!("{:?}", vector2);
    println!("{:?}", vector1_b);
}
```

这个将打印:

```text
[2, 3, 4]
[110, 120, 130]
[10, 20, 30]
```

前两个我们用了一个叫`.map()`的方法。这个方法可以让你对每一个元素做一些事情，然后把它传递下去。最后我们用的是一个叫`.for_each()`的方法。这个方法只是让你对每一个元素做一些事情。`.iter_mut()`加上`for_each()`基本上就是一个`for`的循环。在每一个方法里面，我们可以给每一个元素起一个名字(我们刚才叫它 `x`)，然后用它来改变它。这些被称为闭包，我们将在下一节学习它们。

让我们再来看看它们，一次一个。

首先我们用`.iter()`对`vector1`进行引用。我们给每个元素都加了1，并使其成为一个新的Vec。`vector1`还活着，因为我们只用了引用:我们没有按值取。现在我们有 `vector1`，还有一个新的 Vec 叫 `vector1_a`。因为`.map()`只是传递了它，所以我们需要使用`.collect()`把它变成一个`Vec`。

然后我们用`into_iter`从`vector1`中按值得到一个迭代器。这样就破坏了`vector1`，因为这就是`into_iter()`的作用。所以我们做了`vector1_b`之后，就不能再使用`vector1`了。

最后我们在`vector2`上使用`.iter_mut()`。它是可变的，所以我们不需要使用`.collect()`来创建一个新的Vec。相反，我们用可变引用改变同一Vec中的值。所以`vector2`仍然存在。因为我们不需要一个新的Vec，我们使用`for_each`:它就像一个`for`循环。


### 迭代器如何工作

迭代器的工作原理是使用一个叫做 `.next()` 的方法，它给出一个 `Option`。当你使用迭代器时，Rust会一遍又一遍地调用`next()`。如果得到 `Some`，它就会继续前进。如果得到 `None`，它就停止。

你还记得 `assert_eq!` 宏吗？在文档中，你经常看到它。这里它展示了迭代器的工作原理。

```rust
fn main() {
    let my_vec = vec!['a', 'b', '거', '柳']; // Just a regular Vec

    let mut my_vec_iter = my_vec.iter(); // This is an Iterator type now, but we haven't called it yet

    assert_eq!(my_vec_iter.next(), Some(&'a'));  // Call the first item with .next()
    assert_eq!(my_vec_iter.next(), Some(&'b'));  // Call the next
    assert_eq!(my_vec_iter.next(), Some(&'거')); // Again
    assert_eq!(my_vec_iter.next(), Some(&'柳')); // Again
    assert_eq!(my_vec_iter.next(), None);        // Nothing is left: just None
    assert_eq!(my_vec_iter.next(), None);        // You can keep calling .next() but it will always be None
}
```

为自己的struct或enum实现`Iterator`并不难。首先我们创建一个书库，想一想。

```rust
#[derive(Debug)] // we want to print it with {:?}
struct Library {
    library_type: LibraryType, // this is our enum
    books: Vec<String>, // list of books
}

#[derive(Debug)]
enum LibraryType { // libraries can be city libraries or country libraries
    City,
    Country,
}

impl Library {
    fn add_book(&mut self, book: &str) { // we use add_book to add new books
        self.books.push(book.to_string()); // we take a &str and turn it into a String, then add it to the Vec
    }

    fn new() -> Self { // this creates a new Library
        Self {
            library_type: LibraryType::City, // most are in the city so we'll choose City
                                             // most of the time
            books: Vec::new(),
        }
    }
}

fn main() {
    let mut my_library = Library::new(); // make a new library
    my_library.add_book("The Doom of the Darksword"); // add some books
    my_library.add_book("Demian - die Geschichte einer Jugend");
    my_library.add_book("구운몽");
    my_library.add_book("吾輩は猫である");

    println!("{:?}", my_library.books); // we can print our list of books
}
```

这很好用。现在我们想为库实现`Iterator`，这样我们就可以在`for`循环中使用它。现在如果我们尝试 `for` 循环，它就无法工作。

```rust
for item in my_library {
    println!("{}", item); // ⚠️
}
```

它说:

```text
error[E0277]: `Library` is not an iterator
  --> src\main.rs:47:16
   |
47 |    for item in my_library {
   |                ^^^^^^^^^^ `Library` is not an iterator
   |
   = help: the trait `std::iter::Iterator` is not implemented for `Library`
   = note: required by `std::iter::IntoIterator::into_iter`
```

但是我们可以用`impl Iterator for Library`把库做成迭代器。`Iterator`trait的信息在标准库中。[https://doc.rust-lang.org/std/iter/trait.Iterator.html](https://doc.rust-lang.org/std/iter/trait.Iterator.html)

在页面的左上方写着:`Associated Types: Item`和`Required Methods: next`。"关联类型"的意思是 "一起使用的类型"。我们的关联类型将是`String`，因为我们希望迭代器给我们提供String。

在页面中，它有一个看起来像这样的例子。

```rust
// an iterator which alternates between Some and None
struct Alternate {
    state: i32,
}

impl Iterator for Alternate {
    type Item = i32;

    fn next(&mut self) -> Option<i32> {
        let val = self.state;
        self.state = self.state + 1;

        // if it's even, Some(i32), else None
        if val % 2 == 0 {
            Some(val)
        } else {
            None
        }
    }
}

fn main() {}
```

你可以看到`impl Iterator for Alternate`下面写着`type Item = i32`。这就是关联类型。我们的迭代器将针对我们的书籍列表，这是一个`Vec<String>`。当我们调用next的时候。
 它将给我们一个`String`。所以我们就写`type Item = String;`。这就是关联项。

为了实现 `Iterator`，你需要写 `fn next()` 函数。这是你决定迭代器应该做什么的地方。对于我们的 `Library`，我们首先希望它给我们最后一本书。所以我们将`match`与`.pop()`一起，如果是`Some`的话，就把最后一项去掉。我们还想为每个元素打印 "is found!"。现在它看起来像这样:

```rust
#[derive(Debug, Clone)]
struct Library {
    library_type: LibraryType,
    books: Vec<String>,
}

#[derive(Debug, Clone)]
enum LibraryType {
    City,
    Country,
}

impl Library {
    fn add_book(&mut self, book: &str) {
        self.books.push(book.to_string());
    }

    fn new() -> Self {
        Self {
            library_type: LibraryType::City,
            // most of the time
            books: Vec::new(),
        }
    }
}

impl Iterator for Library {
    type Item = String;

    fn next(&mut self) -> Option<String> {
        match self.books.pop() {
            Some(book) => Some(book + " is found!"), // Rust allows String + &str
            None => None,
        }
    }
}

fn main() {
    let mut my_library = Library::new();
    my_library.add_book("The Doom of the Darksword");
    my_library.add_book("Demian - die Geschichte einer Jugend");
    my_library.add_book("구운몽");
    my_library.add_book("吾輩は猫である");

    for item in my_library.clone() { // we can use a for loop now. Give it a clone so Library won't be destroyed
        println!("{}", item);
    }
}
```

这个打印:

```text
吾輩は猫である is found!
구운몽 is found!
Demian - die Geschichte einer Jugend is found!
The Doom of the Darksword is found!
```

## 闭包

闭包就像快速函数，不需要名字。有时它们被称为lambda。Closures很容易辨识，因为它们使用`||`而不是`()`。它们在 Rust 中非常常见，一旦你学会了使用它们，你就会爱不释手。

你可以将一个闭包绑定到一个变量上，然后当你使用它时，它看起来就像一个函数一样。

```rust
fn main() {
    let my_closure = || println!("This is a closure");
    my_closure();
}
```

所以这个闭包什么都不需要:`||`，并打印一条信息。`This is a closure`.

在`||`之间我们可以添加输入变量和类型，就像在`()`里面添加函数一样。

```rust
fn main() {
    let my_closure = |x: i32| println!("{}", x);

    my_closure(5);
    my_closure(5+5);
}
```

这个打印:

```text
5
10
```

当闭包变得更复杂时，你可以添加一个代码块。那就可以随心所欲的长。

```rust
fn main() {
    let my_closure = || {
        let number = 7;
        let other_number = 10;
        println!("The two numbers are {} and {}.", number, other_number);
          // This closure can be as long as we want, just like a function.
    };

    my_closure();
}
```

但是闭包是特殊的，因为它可以接受闭包之外的变量，即使你只写`||`。所以你可以这样做:

```rust
fn main() {
    let number_one = 6;
    let number_two = 10;

    let my_closure = || println!("{}", number_one + number_two);
    my_closure();
}
```

所以这就打印出了`16`。你不需要在 `||` 中放入任何东西，因为它可以直接取 `number_one` 和 `number_two` 并添加它们。

顺便说一下，这就是**closure**这个名字的由来，因为它们会取变量并将它们 "包围"在里面。如果你想很正确的说。

- 一个`||`如果不把变量从外面包围起来 那就是一个 "匿名函数". 匿名的意思是 "没有名字"。它的工作原理更像一个普通函数。
- `||` 从外部包围变量的函数是 "closure"。它把周围的变量 "封闭"起来使用。

但是人们经常会把所有的`||`函数都叫做闭包，所以你不用担心名字的问题。我们只对任何带有`||`的函数说 "closure"，但请记住，它可能意味着一个 "匿名函数"。

为什么要知道这两者的区别呢？因为匿名函数其实和有名字的函数做的机器代码是一样的。它们给人的感觉是 "高层抽象"，所以有时候大家会觉得机器代码会很复杂。但是Rust用它生成的机器码和普通函数一样快。


所以我们再来看看闭包能做的一些事情。你也可以这样做:

```rust
fn main() {
    let number_one = 6;
    let number_two = 10;

    let my_closure = |x: i32| println!("{}", number_one + number_two + x);
    my_closure(5);
}
```

这个闭包取`number_one`和`number_two`。我们还给了它一个新的变量 `x`，并说 `x` 是 5.然后它把这三个加在一起打印 `21`。

通常在Rust中，你会在一个方法里面看到闭包，因为里面有一个闭包是非常方便的。我们在上一节的 `.map()` 和 `.for_each()` 中看到了闭包。在那一节中，我们写了 `|x|` 来引入迭代器中的下一个元素，这就是一个闭包。

下面再举一个例子:我们知道，如果`unwrap`不起作用，可以用`unwrap_or`方法给出一个值。之前我们写的是:`let fourth = my_vec.get(3).unwrap_or(&0);`。但是还有一个`unwrap_or_else`方法，里面有一个闭包。所以你可以这样做:

```rust
fn main() {
    let my_vec = vec![8, 9, 10];

    let fourth = my_vec.get(3).unwrap_or_else(|| { // try to unwrap. If it doesn't work,
        if my_vec.get(0).is_some() {               // see if my_vec has something at index [0]
            &my_vec[0]                             // Give the number at index 0 if there is something
        } else {
            &0 // otherwise give a &0
        }
    });

    println!("{}", fourth);
}
```

当然，闭包也可以很简单。例如，你可以只写`let fourth = my_vec.get(3).unwrap_or_else(|| &0);`。你不需要总是因为有一个闭包就使用`{}`并写出复杂的代码。只要你把`||`放进去，编译器就知道你放了你需要的闭包。

最常用的闭包方法可能是`.map()`。我们再来看看它。下面是一种使用方法。

```rust
fn main() {
    let num_vec = vec![2, 4, 6];

    let double_vec = num_vec        // take num_vec
        .iter()                     // iterate over it
        .map(|number| number * 2)   // for each item, multiply by two
        .collect::<Vec<i32>>();     // then make a new Vec from this
    println!("{:?}", double_vec);
}
```

另一个很好的例子是在`.enumerate()`之后使用`.for_each()`。`.enumerate()`方法给出一个带有索引号和元素的迭代器。例如:`[10, 9, 8]`变成`(0, 10), (1, 9), (2, 8)`。这里每个项的类型是`(usize, i32)`。所以你可以这样做:

```rust
fn main() {
    let num_vec = vec![10, 9, 8];

    num_vec
        .iter()      // iterate over num_vec
        .enumerate() // get (index, number)
        .for_each(|(index, number)| println!("Index number {} has number {}", index, number)); // do something for each one
}
```

这个将打印:

```text
Index number 0 has number 10
Index number 1 has number 9
Index number 2 has number 8
```

在这种情况下，我们用`for_each`代替`map`。`map`是用于对**每个元素做一些事情，并将其传递出去，而`for_each`是当你看到每个元素**时做一些事情。另外，`map`不做任何事情，除非你使用`collect`这样的方法。

其实，这就是迭代器的有趣之处。如果你尝试`map`而不使用`collect`这样的方法，编译器会告诉你，它什么也不做。它不会崩溃，但编译器会告诉你，你什么都没做。

```rust
fn main() {
    let num_vec = vec![10, 9, 8];

    num_vec
        .iter()
        .enumerate()
        .map(|(index, number)| println!("Index number {} has number {}", index, number));

}
```

它说:

```text
warning: unused `std::iter::Map` that must be used
 --> src\main.rs:4:5
  |
4 | /     num_vec
5 | |         .iter()
6 | |         .enumerate()
7 | |         .map(|(index, number)| println!("Index number {} has number {}", index, number));
  | |_________________________________________________________________________________________^
  |
  = note: `#[warn(unused_must_use)]` on by default
  = note: iterators are lazy and do nothing unless consumed
```

这是一个**警告**，所以这不是一个错误:程序运行正常。但是为什么num_vec没有任何作用呢？我们可以看看类型就知道了。

- `let num_vec = vec![10, 9, 8];` 现在是一个`Vec<i32>`。
- `.iter()` 现在是一个 `Iter<i32>`。所以它是一个迭代器，其元素为 `i32`。

- `.enumerate()`现在是一个`Enumerate<Iter<i32>>`型。所以它是`Enumerate`型的`Iter`型的`i32`。
- `.map()`现在是一个`Map<Enumerate<Iter<i32>>>`的类型。所以它是一个类型`Map`的类型`Enumerate`的类型`Iter`的类型`i32`。

我们所做的只是做了一个越来越复杂的结构。所以这个`Map<Enumerate<Iter<i32>>>`是一个准备好了的结构，但只有当我们告诉它要做什么的时候，它才会去做。Rust这样做是因为它需要保证足够快。它不想这样做:

- 遍历Vec中所有的`i32`
- 然后从迭代器中枚举出所有的`i32`
- 然后将所有列举的`i32`映射过来

Rust 只想做一次计算，所以它创建结构并等待。然后，如果我们说`.collect::<Vec<i32>>()`，它知道该怎么做，并开始移动。这就是`iterators are lazy and do nothing unless consumed`的意思。迭代器在你 "消耗"它们(用完它们)之前不会做任何事情。


你甚至可以用`.collect()`创建像`HashMap`这样复杂的东西，所以它非常强大。下面是一个如何将两个向量放入`HashMap`的例子。首先我们把两个向量创建出来，然后我们会对它们使用`.into_iter()`来得到一个值的迭代器。然后我们使用`.zip()`方法。这个方法将两个迭代器连接在一起，就像拉链一样。最后，我们使用`.collect()`来创建`HashMap`。

下面是代码。

```rust
use std::collections::HashMap;

fn main() {
    let some_numbers = vec![0, 1, 2, 3, 4, 5]; // a Vec<i32>
    let some_words = vec!["zero", "one", "two", "three", "four", "five"]; // a Vec<&str>

    let number_word_hashmap = some_numbers
        .into_iter()                 // now it is an iter
        .zip(some_words.into_iter()) // inside .zip() we put in the other iter. Now they are together.
        .collect::<HashMap<_, _>>();

    println!("For key {} we get {}.", 2, number_word_hashmap.get(&2).unwrap());
}
```

这个将打印:

```text
For key 2 we get two.
```

你可以看到，我们写了 `<HashMap<_, _>>`，因为这足以让 Rust 决定 `HashMap<i32, &str>` 的类型。如果你想写 `.collect::<HashMap<i32, &str>>();`也行，也可以这样写:

```rust
use std::collections::HashMap;

fn main() {
    let some_numbers = vec![0, 1, 2, 3, 4, 5]; // a Vec<i32>
    let some_words = vec!["zero", "one", "two", "three", "four", "five"]; // a Vec<&str>
    let number_word_hashmap: HashMap<_, _> = some_numbers  // Because we tell it the type here...
        .into_iter()
        .zip(some_words.into_iter())
        .collect(); // we don't have to tell it here
}
```

还有一种方法，就像`.enumerate()`的`char`。`char_indices()`. (Indices的意思是 "索引")。你用它的方法是一样的。假设我们有一个由3位数组成的大字符串。

```rust
fn main() {
    let numbers_together = "140399923481800622623218009598281";

    for (index, number) in numbers_together.char_indices() {
        match (index % 3, number) {
            (0..=1, number) => print!("{}", number), // just print the number if there is a remainder
            _ => print!("{}\t", number), // otherwise print the number with a tab space
        }
    }
}
```

打印`140     399     923     481     800     622     623     218     009     598    281`。


### 闭包中的|_|

有时你会在一个闭包中看到 `|_|`。这意味着这个闭包需要一个参数(比如 `x`)，但你不想使用它。所以 `|_|` 意味着 "好吧，这个闭包需要一个参数，但我不会给它一个名字，因为我不关心它"。

下面是一个错误的例子，当你不这样做的时候。

```rust
fn main() {
    let my_vec = vec![8, 9, 10];

    println!("{:?}", my_vec.iter().for_each(|| println!("We didn't use the variables at all"))); // ⚠️
}
```

Rust说

```text
error[E0593]: closure is expected to take 1 argument, but it takes 0 arguments
  --> src\main.rs:28:36
   |
28 |     println!("{:?}", my_vec.iter().for_each(|| println!("We didn't use the variables at all")));
   |                                    ^^^^^^^^ -- takes 0 arguments
   |                                    |
   |                                    expected closure that takes 1 argument
```

编译器其实给你一些帮助。

```text
help: consider changing the closure to take and ignore the expected argument
   |
28 |     println!("{:?}", my_vec.iter().for_each(|_| println!("We didn't use the variables at all")));
```

这是很好的建议。如果你把`||`改成`|_|`就可以了。

### 闭包和迭代器的有用方法

一旦你熟悉了闭包，Rust就会成为一种非常有趣的语言。有了闭包，你可以将方法互相*链接*起来，用很少的代码做很多事情。下面是一些我们还没有见过的闭包和使用闭包的方法。

`.filter()`: 这可以让你在迭代器中保留你想保留的元素。让我们过滤一年中的月份。

```rust
fn main() {
    let months = vec!["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];

    let filtered_months = months
        .into_iter()                         // make an iter
        .filter(|month| month.len() < 5)     // We don't want months more than 5 bytes in length.
                                             // We know that each letter is one byte so .len() is fine
        .filter(|month| month.contains("u")) // Also we only like months with the letter u
        .collect::<Vec<&str>>();

    println!("{:?}", filtered_months);
}
```

这个打印`["June", "July"]`。



`.filter_map()`. 这个叫做`filter_map()`，因为它做了`.filter()`和`.map()`。闭包必须返回一个 `Option<T>`，然后对每个`Option`, 如果是 `Some`, `filter_map()`将取出它的值。所以比如说你`.filter_map()`一个`vec![Some(2), None, Some(3)]`，它就会返回`[2, 3]`。

我们将用一个`Company`结构体来写一个例子。每个公司都有一个`name`，所以这个字段是`String`，但是CEO可能最近已经辞职了。所以`ceo`字段是`Option<String>`。我们会`.filter_map()`过一些公司，只保留CEO名字。

```rust
struct Company {
    name: String,
    ceo: Option<String>,
}

impl Company {
    fn new(name: &str, ceo: &str) -> Self {
        let ceo = match ceo {
            "" => None,
            name => Some(name.to_string()),
        }; // ceo is decided, so now we return Self
        Self {
            name: name.to_string(),
            ceo,
        }
    }

    fn get_ceo(&self) -> Option<String> {
        self.ceo.clone() // Just returns a clone of the CEO (struct is not Copy)
    }
}

fn main() {
    let company_vec = vec![
        Company::new("Umbrella Corporation", "Unknown"),
        Company::new("Ovintiv", "Doug Suttles"),
        Company::new("The Red-Headed League", ""),
        Company::new("Stark Enterprises", ""),
    ];

    let all_the_ceos = company_vec
        .into_iter()
        .filter_map(|company| company.get_ceo()) // filter_map needs Option<T>
        .collect::<Vec<String>>();

    println!("{:?}", all_the_ceos);
}
```

这就打印出了`["Unknown", "Doug Suttles"]`。

既然 `.filter_map()` 需要 `Option`，那么 `Result` 呢？没问题:有一个叫做 `.ok()` 的方法，可以把 `Result` 变成 `Option`。之所以叫`.ok()`，是因为它能发送的只是`Ok`的结果(`Err`的信息没有了)。你记得`Option`是`Option<T>`，而`Result`是`Result<T, E>`，同时有`Ok`和`Err`的信息。所以当你使用`.ok()`时，任何`Err`的信息都会丢失，变成`None`。

使用 `.parse()` 是一个很简单的例子，我们尝试解析一些用户输入。`.parse()`在这里接受一个`&str`，并试图把它变成一个`f32`。它返回一个 `Result`，但我们使用的是 `filter_map()`，所以我们只需抛出错误。`Err`的任何内容都会变成`None`，并被`.filter_map()`过滤掉。

```rust
fn main() {
    let user_input = vec!["8.9", "Nine point nine five", "8.0", "7.6", "eleventy-twelve"];

    let actual_numbers = user_input
        .into_iter()
        .filter_map(|input| input.parse::<f32>().ok())
        .collect::<Vec<f32>>();

    println!("{:?}", actual_numbers);
}
```

将打印: `[8.9, 8.0, 7.6]`。

与`.ok()`相对的是`.ok_or()`和`ok_or_else()`。这样就把`Option`变成了`Result`。之所以叫`.ok_or()`，是因为`Result`给出了一个`Ok`**或**`Err`，所以你必须让它知道`Err`的值是多少。这是因为`None`中的`Option`没有任何信息。另外，你现在可以看到，这些方法名称中的*else*部分意味着它有一个闭包。

我们可以把我们的`Option`从`Company`结构中取出来，然后这样把它变成一个`Result`。对于长期的错误处理，最好是创建自己的错误类型。
 但是现在我们只是给它一个错误信息，所以它就变成了`Result<String, &str>`。

```rust
// Everything before main() is exactly the same
struct Company {
    name: String,
    ceo: Option<String>,
}

impl Company {
    fn new(name: &str, ceo: &str) -> Self {
        let ceo = match ceo {
            "" => None,
            name => Some(name.to_string()),
        };
        Self {
            name: name.to_string(),
            ceo,
        }
    }

    fn get_ceo(&self) -> Option<String> {
        self.ceo.clone()
    }
}

fn main() {
    let company_vec = vec![
        Company::new("Umbrella Corporation", "Unknown"),
        Company::new("Ovintiv", "Doug Suttles"),
        Company::new("The Red-Headed League", ""),
        Company::new("Stark Enterprises", ""),
    ];

    let mut results_vec = vec![]; // Pretend we need to gather error results too

    company_vec
        .iter()
        .for_each(|company| results_vec.push(company.get_ceo().ok_or("No CEO found")));

    for item in results_vec {
        println!("{:?}", item);
    }
}
```

这行是最大的变化:

```rust
// 🚧
.for_each(|company| results_vec.push(company.get_ceo().ok_or("No CEO found")));
```

它的意思是:"每家公司，用`get_ceo()`. 如果你得到了，那就把`Ok`里面的数值传给你。如果没有，就在`Err`里面传递 "没有找到CEO"。然后把这个推到vec里。"

所以当我们打印`results_vec`的时候，就会得到这样的结果。

```text
Ok("Unknown")
Ok("Doug Suttles")
Err("No CEO found")
Err("No CEO found")
```

所以现在我们有了所有四个条目。现在让我们使用 `.ok_or_else()`，这样我们就可以使用一个闭包，并得到一个更好的错误信息。现在我们有空间使用`format!`来创建一个`String`，并将公司名称放在其中。然后我们返回`String`。

```rust
// Everything before main() is exactly the same
struct Company {
    name: String,
    ceo: Option<String>,
}

impl Company {
    fn new(name: &str, ceo: &str) -> Self {
        let ceo = match ceo {
            "" => None,
            name => Some(name.to_string()),
        };
        Self {
            name: name.to_string(),
            ceo,
        }
    }

    fn get_ceo(&self) -> Option<String> {
        self.ceo.clone()
    }
}

fn main() {
    let company_vec = vec![
        Company::new("Umbrella Corporation", "Unknown"),
        Company::new("Ovintiv", "Doug Suttles"),
        Company::new("The Red-Headed League", ""),
        Company::new("Stark Enterprises", ""),
    ];

    let mut results_vec = vec![];

    company_vec.iter().for_each(|company| {
        results_vec.push(company.get_ceo().ok_or_else(|| {
            let err_message = format!("No CEO found for {}", company.name);
            err_message
        }))
    });

    for item in results_vec {
        println!("{:?}", item);
    }
}
```

这样一来，我们就有了。

```text
Ok("Unknown")
Ok("Doug Suttles")
Err("No CEO found for The Red-Headed League")
Err("No CEO found for Stark Enterprises")
```


`.and_then()`是一个有用的方法，它接收一个`Option`，然后让你对它的值做一些事情，并把它传递出去。所以它的输入是一个 `Option`，输出也是一个 `Option`。这有点像一个安全的 "解包，然后做一些事情，然后再包"。

一个简单的例子是，我们使用 `.get()` 从一个 vec 中得到一个数字，因为它返回一个 `Option`。现在我们可以把它传给 `and_then()`，如果它是 `Some`，我们可以对它做一些数学运算。如果是`None`，那么`None`就会被传递过去。

```rust
fn main() {
    let new_vec = vec![8, 9, 0]; // just a vec with numbers

    let number_to_add = 5;       // use this in the math later
    let mut empty_vec = vec![];  // results go in here


    for index in 0..5 {
        empty_vec.push(
            new_vec
               .get(index)
                .and_then(|number| Some(number + 1))
                .and_then(|number| Some(number + number_to_add))
        );
    }
    println!("{:?}", empty_vec);
}
```

这就打印出了`[Some(14), Some(15), Some(6), None, None]`。你可以看到`None`并没有被过滤掉，只是传递了。




`.and()`有点像`Option`的`bool`。你可以匹配很多个`Option`，如果它们都是`Some`，那么它会给出最后一个。而如果其中一个是`None`，那么就会给出`None`。

首先这里有一个`bool`的例子来帮助想象。你可以看到，如果你用的是`&&`(和)，哪怕是一个`false`，也会让一切`false`。

```rust
fn main() {
    let one = true;
    let two = false;
    let three = true;
    let four = true;

    println!("{}", one && three); // prints true
    println!("{}", one && two && three && four); // prints false
}
```

现在这里的`.and()`也是一样的。想象一下，我们做了五次操作，并把结果放在一个Vec<Option<&str>>中。如果我们得到一个值，我们就把`Some("success!")`推到Vec中。然后我们再做两次这样的操作。之后我们用`.and()`每次只显示得到`Some`的索引。

```rust
fn main() {
    let first_try = vec![Some("success!"), None, Some("success!"), Some("success!"), None];
    let second_try = vec![None, Some("success!"), Some("success!"), Some("success!"), Some("success!")];
    let third_try = vec![Some("success!"), Some("success!"), Some("success!"), Some("success!"), None];

    for i in 0..first_try.len() {
        println!("{:?}", first_try[i].and(second_try[i]).and(third_try[i]));
    }
}
```

这个打印:

```text
None
None
Some("success!")
Some("success!")
None
```

第一个(索引0)是`None`，因为在`second_try`中有一个`None`为索引0。第二个是`None`，因为在`first_try`中有一个`None`。其次是`Some("success!")`，因为`first_try`、`second try`、`third_try`中没有`None`。



`.any()`和`.all()`在迭代器中非常容易使用。它们根据你的输入返回一个`bool`。在这个例子中，我们做了一个非常大的vec(大约20000个元素)，包含了从`'a'`到`'働'`的所有字符。然后我们创建一个函数来检查是否有字符在其中。

接下来我们创建一个更小的vec，问它是否都是字母(用`.is_alphabetic()`方法)。然后我们问它是不是所有的字符都小于韩文字符`'행'`。

还要注意放一个参照物，因为`.iter()`给了一个参照物，你需要一个`&`和另一个`&`进行比较。

```rust
fn in_char_vec(char_vec: &Vec<char>, check: char) {
    println!("Is {} inside? {}", check, char_vec.iter().any(|&char| char == check));
}

fn main() {
    let char_vec = ('a'..'働').collect::<Vec<char>>();
    in_char_vec(&char_vec, 'i');
    in_char_vec(&char_vec, '뷁');
    in_char_vec(&char_vec, '鑿');

    let smaller_vec = ('A'..'z').collect::<Vec<char>>();
    println!("All alphabetic? {}", smaller_vec.iter().all(|&x| x.is_alphabetic()));
    println!("All less than the character 행? {}", smaller_vec.iter().all(|&x| x < '행'));
}
```

这个打印:

```text
Is i inside? true
Is 뷁 inside? false
Is 鑿 inside? false
All alphabetic? false
All less than the character 행? true
```

顺便说一下，`.any()`只检查到一个匹配的元素，然后就停止了。如果它已经找到了一个匹配项，它不会检查所有的元素。如果您要在 `Vec` 上使用 `.any()`，最好把可能匹配的元素推到前面。或者你可以在 `.iter()` 之后使用 `.rev()` 来反向迭代。这里有一个这样的vec。

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);
}
```

所以这个`Vec`有1000个`6`，后面还有一个`5`。我们假设我们要用`.any()`来看看它是否包含5。首先让我们确定`.rev()`是有效的。记住，一个`Iterator`总是有`.next()`，让你每次都检查它的工作。

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);

    let mut iterator = big_vec.iter().rev();
    println!("{:?}", iterator.next());
    println!("{:?}", iterator.next());
}
```

它的打印。

```text
Some(5)
Some(6)
```

我们是对的:有一个`Some(5)`，然后1000个`Some(6)`开始。所以我们可以这样写。

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);

    println!("{:?}", big_vec.iter().rev().any(|&number| number == 5));
}
```

而且因为是`.rev()`，所以它只调用`.next()`一次就停止了。如果我们不用`.rev()`，那么它将调用`.next()` 1001次才停止。这段代码显示了它。

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);

    let mut counter = 0; // Start counting
    let mut big_iter = big_vec.into_iter(); // Make it an Iterator

    loop {
        counter +=1;
        if big_iter.next() == Some(5) { // Keep calling .next() until we get Some(5)
            break;
        }
    }
    println!("Final counter is: {}", counter);
}
```

这将打印出 `Final counter is: 1001`，所以我们知道它必须调用 `.next()` 1001 次才能找到 5。




`.find()` 告诉你一个迭代器是否有东西，而 `.position()` 告诉你它在哪里。`.find()`与`.any()`不同，因为它返回一个`Option`，里面有值(或`None`)。同时，`.position()`也是一个带有位置号的`Option`，或`None`。换句话说

- `.find()`: "我尽量帮你拿"
- `.position()`:"我帮你找找看在哪里"

下面是一个简单的例子。

```rust
fn main() {
    let num_vec = vec![10, 20, 30, 40, 50, 60, 70, 80, 90, 100];

    println!("{:?}", num_vec.iter().find(|&number| number % 3 == 0)); // find takes a reference, so we give it &number
    println!("{:?}", num_vec.iter().find(|&number| number * 2 == 30));

    println!("{:?}", num_vec.iter().position(|&number| number % 3 == 0));
    println!("{:?}", num_vec.iter().position(|&number| number * 2 == 30));

}
```

这个打印:

```text
Some(30) // This is the number itself
None // No number inside times 2 == 30
Some(2) // This is the position
None
```



使用 `.cycle()` 你可以创建一个永远循环的迭代器。这种类型的迭代器与 `.zip()` 很好地结合在一起，可以创建新的东西，就像这个例子，它创建了一个 `Vec<(i32, &str)>`。

```rust
fn main() {
    let even_odd = vec!["even", "odd"];

    let even_odd_vec = (0..6)
        .zip(even_odd.into_iter().cycle())
        .collect::<Vec<(i32, &str)>>();
    println!("{:?}", even_odd_vec);
}
```

所以，即使`.cycle()`可能永远不会结束，但当把它们压缩在一起时，另一个迭代器只运行了6次。
 也就是说，`.cycle()`所做的迭代器不会再被`.next()`调用，所以六次之后就完成了。输出的结果是

```
[(0, "even"), (1, "odd"), (2, "even"), (3, "odd"), (4, "even"), (5, "odd")]
```

类似的事情也可以用一个没有结尾的范围来完成。如果你写`0..`，那么你就创建了一个永不停止的范围。你可以很容易地使用这个方法。

```rust
fn main() {
    let ten_chars = ('a'..).take(10).collect::<Vec<char>>();
    let skip_then_ten_chars = ('a'..).skip(1300).take(10).collect::<Vec<char>>();

    println!("{:?}", ten_chars);
    println!("{:?}", skip_then_ten_chars);
}
```

两者都是打印十个字符，但第二个跳过1300位，打印的是亚美尼亚语的十个字母。

```
['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
['յ', 'ն', 'շ', 'ո', 'չ', 'պ', 'ջ', 'ռ', 'ս', 'վ']
```


另一种流行的方法叫做`.fold()`。这个方法经常用于将迭代器中的元素加在一起，但你也可以做更多的事情。它与`.for_each()`有些类似。在 `.fold()` 中，你首先添加一个起始值 (如果你是把元素加在一起，那么就是 0)，然后是一个逗号，然后是闭包。结尾给你两个元素:到目前为止的总数，和下一个元素。首先这里有一个简单的例子，显示`.fold()`将元素加在一起。

```rust
fn main() {
    let some_numbers = vec![9, 6, 9, 10, 11];

    println!("{}", some_numbers
        .iter()
        .fold(0, |total_so_far, next_number| total_so_far + next_number)
    );
}
```

所以，在第1步中，它从0开始，再加上下一个数字:9。

- 第1步，从0开始，加上下一个数字9
- 然后把9加上6: 15。
- 然后把15加上9: 24。
- 然后取24，再加上10: 34。
- 最后取34，再加上11: 45。所以它的打印结果是`45`.


但是你不需要只用它来添加东西。下面是一个例子，我们在每一个字符上加一个'-'，就会变成`String`。

```rust
fn main() {
    let a_string = "I don't have any dashes in me.";

    println!(
        "{}",
        a_string
            .chars() // Now it's an iterator
            .fold("-".to_string(), |mut string_so_far, next_char| { // Start with a String "-". Bring it in as mutable each time along with the next char
                string_so_far.push(next_char); // Push the char on, then '-'
                string_so_far.push('-');
                string_so_far} // Don't forget to pass it on to the next loop
            ));
}
```

这个打印:

```text
-I- -d-o-n-'-t- -h-a-v-e- -a-n-y- -d-a-s-h-e-s- -i-n- -m-e-.-
```



还有很多其他方便的方法，比如

- `.take_while()`，只要得到`true`，就会带入一个迭代器(例如`take while x > 5`)
- `.cloned()`，它在迭代器内做了一个克隆。这将一个引用变成了一个值。
- `.by_ref()`，它使迭代器取一个引用。这很好的保证了你使用`Vec`或类似的方法来创建迭代器后可以使用它。
- 许多其他的`_while`方法:`.skip_while()`、`.map_while()`等等。
- `.sum()`:就是把所有的东西加在一起。



`.chunks()`和`.windows()`是将矢量切割成你想要的尺寸的两种方法。你把你想要的尺寸放在括号里。比如说你有一个有10个元素的矢量，你想要一个3的尺寸，它的工作原理是这样的。

- `.chunks()`会给你4个切片: [0, 1, 2], 然后是[3, 4, 5], 然后是[6, 7, 8], 最后是[9]. 所以它会尝试用三个元素创建一个切片，但如果它没有三个元素，那么它就不会崩溃。它只会给你剩下的东西。

- `.windows()`会先给你一个[0, 1, 2]的切片。然后它将移过一片，给你[1, 2, 3]。它将一直这样做，直到最后到达3的最后一片，然后停止。

所以让我们在一个简单的数字向量上使用它们。它看起来像这样:

```rust
fn main() {
    let num_vec = vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 0];

    for chunk in num_vec.chunks(3) {
        println!("{:?}", chunk);
    }
    println!();
    for window in num_vec.windows(3) {
        println!("{:?}", window);
    }
}
```

这个打印:

```text
[1, 2, 3]
[4, 5, 6]
[7, 8, 9]
[0]

[1, 2, 3]
[2, 3, 4]
[3, 4, 5]
[4, 5, 6]
[5, 6, 7]
[6, 7, 8]
[7, 8, 9]
[8, 9, 0]
```

顺便说一下，如果你什么都不给它，`.chunks()`会崩溃。你可以为一个只有一项的向量写`.chunks(1000)`，但你不能为任何长度为0的东西写`.chunks()`。 如果你点击[src]，你可以在函数中看到这一点，因为它说`assert!(chunk_size != 0);`。



`.match_indices()` 让你把 `String` 或 `&str` 里面所有符合你的输入的东西都提取出来，并给你索引。它与 `.enumerate()` 类似，因为它返回一个包含两个元素的元组。

```rust
fn main() {
    let rules = "Rule number 1: No fighting. Rule number 2: Go to bed at 8 pm. Rule number 3: Wake up at 6 am.";
    let rule_locations = rules.match_indices("Rule").collect::<Vec<(_, _)>>(); // This is Vec<usize, &str> but we just tell Rust to do it
    println!("{:?}", rule_locations);
}
```

这个打印:

```text
[(0, "Rule"), (28, "Rule"), (62, "Rule")]
```



`.peekable()` 让你创建一个迭代器，在那里你可以看到 (窥视) 下一个元素。它就像调用 `.next()` (它给出了一个 `Option`)，除了迭代器不会移动，所以你可以随意使用它。实际上，你可以把peekable看成是 "可停止"的，因为你可以想停多久就停多久。下面是一个例子，我们对每个元素都使用`.peek()`三次。我们可以永远使用`.peek()`，直到我们使用`.next()`移动到下一个元素。

```rust
fn main() {
    let just_numbers = vec![1, 5, 100];
    let mut number_iter = just_numbers.iter().peekable(); // This actually creates a type of iterator called Peekable

    for _ in 0..3 {
        println!("I love the number {}", number_iter.peek().unwrap());
        println!("I really love the number {}", number_iter.peek().unwrap());
        println!("{} is such a nice number", number_iter.peek().unwrap());
        number_iter.next();
    }
}
```

这个打印:

```text
I love the number 1
I really love the number 1
1 is such a nice number
I love the number 5
I really love the number 5
5 is such a nice number
I love the number 100
I really love the number 100
100 is such a nice number
```

下面是另一个例子，我们使用`.peek()`对一个元素进行匹配。使用完后，我们调用`.next()`。


```rust
fn main() {
    let locations = vec![
        ("Nevis", 25),
        ("Taber", 8428),
        ("Markerville", 45),
        ("Cardston", 3585),
    ];
    let mut location_iter = locations.iter().peekable();
    while location_iter.peek().is_some() {
        match location_iter.peek() {
            Some((name, number)) if *number < 100 => { // .peek() gives us a reference so we need *
                println!("Found a hamlet: {} with {} people", name, number)
            }
            Some((name, number)) => println!("Found a town: {} with {} people", name, number),
            None => break,
        }
        location_iter.next();
    }
}
```

这个打印:

```text
Found a hamlet: Nevis with 25 people
Found a town: Taber with 8428 people
Found a hamlet: Markerville with 45 people
Found a town: Cardston with 3585 people
```

最后，这里有一个例子，我们也使用`.match_indices()`。在这个例子中，我们根据`&str`中的空格数，将名字放入`struct`中。

```rust
#[derive(Debug)]
struct Names {
    one_word: Vec<String>,
    two_words: Vec<String>,
    three_words: Vec<String>,
}

fn main() {
    let vec_of_names = vec![
        "Caesar",
        "Frodo Baggins",
        "Bilbo Baggins",
        "Jean-Luc Picard",
        "Data",
        "Rand Al'Thor",
        "Paul Atreides",
        "Barack Hussein Obama",
        "Bill Jefferson Clinton",
    ];

    let mut iter_of_names = vec_of_names.iter().peekable();

    let mut all_names = Names { // start an empty Names struct
        one_word: vec![],
        two_words: vec![],
        three_words: vec![],
    };

    while iter_of_names.peek().is_some() {
        let next_item = iter_of_names.next().unwrap(); // We can use .unwrap() because we know it is Some
        match next_item.match_indices(' ').collect::<Vec<_>>().len() { // Create a quick vec using .match_indices and check the length
            0 => all_names.one_word.push(next_item.to_string()),
            1 => all_names.two_words.push(next_item.to_string()),
            _ => all_names.three_words.push(next_item.to_string()),
        }
    }

    println!("{:?}", all_names);
}
```

这将打印:

```text
Names { one_word: ["Caesar", "Data"], two_words: ["Frodo Baggins", "Bilbo Baggins", "Jean-Luc Picard", "Rand Al\'Thor", "Paul Atreides"], three_words:
["Barack Hussein Obama", "Bill Jefferson Clinton"] }
```


## dbg! 宏和.inspect

`dbg!`是一个非常有用的宏，可以快速打印信息。它是 `println!` 的一个很好的替代品，因为它的输入速度更快，提供的信息更多。

```rust
fn main() {
    let my_number = 8;
    dbg!(my_number);
}
```

这样就可以打印出`[src\main.rs:4] my_number = 8`。

但实际上，你可以把`dbg!`放在其他很多地方，甚至可以把代码包在里面。比如看这段代码。

```rust
fn main() {
    let mut my_number = 9;
    my_number += 10;

    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec.iter().map(|x| x * 2).collect::<Vec<i32>>();
}
```

这段代码创建了一个新的可变数字，并改变了它。然后创建一个vec，并使用`iter`和`map`以及`collect`创建一个新的vec。在这段代码中，我们几乎可以把`dbg!`放在任何地方。`dbg!`问编译器："此刻你在做什么？"，然后告诉你:

```rust
fn main() {
    let mut my_number = dbg!(9);
    dbg!(my_number += 10);

    let new_vec = dbg!(vec![8, 9, 10]);

    let double_vec = dbg!(new_vec.iter().map(|x| x * 2).collect::<Vec<i32>>());

    dbg!(double_vec);
}
```

所以这个打印:

```text
[src\main.rs:3] 9 = 9
```

和：

```text
[src\main.rs:4] my_number += 10 = ()
```

和：

```text
[src\main.rs:6] vec![8, 9, 10] = [
    8,
    9,
    10,
]
```

而这个，甚至可以显示出表达式的值。

```text
[src\main.rs:8] new_vec.iter().map(|x| x * 2).collect::<Vec<i32>>() = [
    16,
    18,
    20,
]
```

和：

```text
[src\main.rs:10] double_vec = [
    16,
    18,
    20,
]
```


`.inspect` 与 `dbg!` 有点类似，就像在迭代器中使用`map`一样使用它。它给了你迭代项，你可以打印它或者做任何你想做的事情。例如，我们再看看我们的 `double_vec`。

```rust
fn main() {
    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec
        .iter()
        .map(|x| x * 2)
        .collect::<Vec<i32>>();
}
```

我们想知道更多关于代码的信息。所以我们在两个地方添加`inspect()`。

```rust
fn main() {
    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec
        .iter()
        .inspect(|first_item| println!("The item is: {}", first_item))
        .map(|x| x * 2)
        .inspect(|next_item| println!("Then it is: {}", next_item))
        .collect::<Vec<i32>>();
}
```

这个打印:

```text
The item is: 8
Then it is: 16
The item is: 9
Then it is: 18
The item is: 10
Then it is: 20
```

而且因为`.inspect`采取的是封闭式，所以我们可以随意写。

```rust
fn main() {
    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec
        .iter()
        .inspect(|first_item| {
            println!("The item is: {}", first_item);
            match **first_item % 2 { // first item is a &&i32 so we use **
                0 => println!("It is even."),
                _ => println!("It is odd."),
            }
            println!("In binary it is {:b}.", first_item);
        })
        .map(|x| x * 2)
        .collect::<Vec<i32>>();
}
```

这个打印:

```text
The item is: 8
It is even.
In binary it is 1000.
The item is: 9
It is odd.
In binary it is 1001.
The item is: 10
It is even.
In binary it is 1010.
```

## &str的类型

`&str`的类型不止一种。我们有。

- 字符串： 当你写`let my_str = "I am a &str"`的时候，你就会产生这些字符。它们在整个程序中持续存在，因为它们是直接写进二进制中的，它们的类型是 `&'static str`。`'`的意思是它的生命期，字符串字元有一个叫`static`的生命期。
- 借用str：这是常规的 `&str` 形式，没有 `static` 生命期。如果你创建了一个`String`，并得到了它的引用，当你需要它时，Rust会把它转换为`&str`。比如说

```rust
fn prints_str(my_str: &str) { // it can use &String like a &str
    println!("{}", my_str);
}

fn main() {
    let my_string = String::from("I am a string");
    prints_str(&my_string); // we give prints_str a &String
}
```

那么什么是lifetime呢？我们现在就来了解一下。

## 生命期

生命期的意思是 "变量的生命期有多长"。你只需要考虑引用的生命期。这是因为引用的生命期不能比它们来自的对象更长。例如，这个函数就不能用。

```rust
fn returns_reference() -> &str {
    let my_string = String::from("I am a string");
    &my_string // ⚠️
}

fn main() {}
```

问题是`my_string`只存在于`returns_reference`中。我们试图返回 `&my_string`，但是 `&my_string` 不能没有 `my_string`。所以编译器说不行。

这个代码也不行。

```rust
fn returns_str() -> &str {
    let my_string = String::from("I am a string");
    "I am a str" // ⚠️
}

fn main() {
    let my_str = returns_str();
    println!("{}", my_str);
}
```

但几乎是成功的。编译器说:

```text
error[E0106]: missing lifetime specifier
 --> src\main.rs:6:21
  |
6 | fn returns_str() -> &str {
  |                     ^ expected named lifetime parameter
  |
  = help: this function's return type contains a borrowed value, but there is no value for it to be borrowed from
help: consider using the `'static` lifetime
  |
6 | fn returns_str() -> &'static str {
  |                     ^^^^^^^^
```

`missing lifetime specifier`的意思是，我们需要加一个`'`的生命期。然后说它`contains a borrowed value, but there is no value for it to be borrowed from`。也就是说，`I am a str`不是借来的。它写`&'static str`就说`consider using the 'static lifetime`。所以它认为我们应该尝试说这是一个字符串的文字。

现在它工作了。

```rust
fn returns_str() -> &'static str {
    let my_string = String::from("I am a string");
    "I am a str"
}

fn main() {
    let my_str = returns_str();
    println!("{}", my_str);
}
```

这是因为我们返回了一个 `&str`，生命期为 `static`。同时，`my_string`只能以`String`的形式返回:我们不能返回对它的引用，因为它将在下一行死亡。

所以现在`fn returns_str() -> &'static str`告诉Rust， "别担心，我们只会返回一个字符串字面量". 字符串字面量在整个程序中都是有效的，所以Rust很高兴。你会注意到，这与泛型类似。当我们告诉编译器类似 `<T: Display>` 的东西时，我们承诺我们将只使用实现了 `Display` 的输入。生命期也类似:我们并没有改变任何变量的生命期。我们只是告诉编译器输入的生命期是多少。

但是`'static`并不是唯一的生命期。实际上，每个变量都有一个生命期，但通常我们不必写出来。编译器很聪明，一般都能自己算出来。只有在编译器不知道的时候，我们才需要写出生命期。

下面是另一个生命期的例子。想象一下，我们想创建一个`City`结构，并给它一个`&str`的名字。我们可能想这样做，因为这样做的性能比用`String`快。所以我们这样写，但还不能用。

```rust
#[derive(Debug)]
struct City {
    name: &str, // ⚠️
    date_founded: u32,
}

fn main() {
    let my_city = City {
        name: "Ichinomiya",
        date_founded: 1921,
    };
}
```

编译器说:

```text
error[E0106]: missing lifetime specifier
 --> src\main.rs:3:11
  |
3 |     name: &str,
  |           ^ expected named lifetime parameter
  |
help: consider introducing a named lifetime parameter
  |
2 | struct City<'a> {
3 |     name: &'a str,
  |
```

Rust 需要 `&str` 的生命期，因为 `&str` 是一个引用。如果`name`指向的值被丢弃了会怎样？那就不安全了。

`'static`呢，能用吗？我们以前用过。我们试试吧。

```rust
#[derive(Debug)]
struct City {
    name: &'static str, // change &str to &'static str
    date_founded: u32,
}

fn main() {
    let my_city = City {
        name: "Ichinomiya",
        date_founded: 1921,
    };

    println!("{} was founded in {}", my_city.name, my_city.date_founded);
}
```

好的，这就可以了。也许这就是你想要的结构。但是，请注意，我们只能接受 "字符串字面量"，所以不能接受对其他东西的引用。所以这将无法工作。

```rust
#[derive(Debug)]
struct City {
    name: &'static str, // must live for the whole program
    date_founded: u32,
}

fn main() {
    let city_names = vec!["Ichinomiya".to_string(), "Kurume".to_string()]; // city_names does not live for the whole program

    let my_city = City {
        name: &city_names[0], // ⚠️ This is a &str, but not a &'static str. It is a reference to a value inside city_names
        date_founded: 1921,
    };

    println!("{} was founded in {}", my_city.name, my_city.date_founded);
}
```

编译器说:

```text
error[E0597]: `city_names` does not live long enough
  --> src\main.rs:12:16
   |
12 |         name: &city_names[0],
   |                ^^^^^^^^^^
   |                |
   |                borrowed value does not live long enough
   |                requires that `city_names` is borrowed for `'static`
...
18 | }
   | - `city_names` dropped here while still borrowed
```

这一点很重要，因为我们给它的引用其实已经够长寿了。但是我们承诺只给它一个`&'static str`，这就是问题所在。

所以现在我们就试试之前编译器的建议。它说尝试写`struct City<'a>`和`name: &'a str`。这就意味着，只有当`name`活到`City`一样寿命的情况下，它才会接受`name`的引用。

```rust
#[derive(Debug)]
struct City<'a> { // City has lifetime 'a
    name: &'a str, // and name also has lifetime 'a.
    date_founded: u32,
}

fn main() {
    let city_names = vec!["Ichinomiya".to_string(), "Kurume".to_string()];

    let my_city = City {
        name: &city_names[0],
        date_founded: 1921,
    };

    println!("{} was founded in {}", my_city.name, my_city.date_founded);
}
```

另外记住，如果你愿意，你可以写任何东西来代替`'a`。这也和泛型类似，我们写`T`和`U`，但实际上可以写任何东西。

```rust
#[derive(Debug)]
struct City<'city> { // The lifetime is now called 'city
    name: &'city str, // and name has the 'city lifetime
    date_founded: u32,
}

fn main() {}
```

所以一般都会写`'a, 'b, 'c`等，因为这样写起来比较快，也是常用的写法。但如果你想的话，你可以随时更改。有一个很好的建议是，如果代码非常复杂，把生命期改成一个 "人类可读"的名字可以帮助你阅读代码。

我们再来看看与trait的比较，对于泛型。比如说

```rust
use std::fmt::Display;

fn prints<T: Display>(input: T) {
    println!("T is {}", input);
}

fn main() {}
```

当你写`T: Display`的时候，它的意思是 "只有当T有Display时，才取T"。
而不是说: "我把Display给T".

对于生命期也是如此。当你在这里写 'a:

```rust
#[derive(Debug)]
struct City<'a> {
    name: &'a str,
    date_founded: u32,
}

fn main() {}
```

意思是 "如果`name`的生命期至少与`City`一样长，才接受`name`的输入"。
它的意思不是说: "我会让`name`的输入与`City`一样长寿"。


现在我们可以了解一下之前看到的`<'_>`。这被称为 "匿名生命期"，是使用引用的一个指标。例如，当你在实现结构时，Rust会向你建议使用。这里有一个几乎可以工作的结构体，但还不能工作：

```rust
    // ⚠️
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

fn main() {}
```

所以我们对`struct`做了我们需要做的事情:首先我们说`name`来自于一个`&str`。这就意味着我们需要lifetime，所以我们给了它`<'a>`。然后我们必须对`struct`做同样的处理，以证明它们至少和这个生命期一样长。但是Rust却告诉我们要这样做:

```text
error[E0726]: implicit elided lifetime not allowed here
 --> src\main.rs:6:6
  |
6 | impl Adventurer {
  |      ^^^^^^^^^^- help: indicate the anonymous lifetime: `<'_>`
```

它想让我们加上那个匿名的生命期，以表明有一个引用被使用。所以如果我们这样写，它就会很高兴。

```rust
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer<'_> {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

fn main() {}
```

这个生命期是为了让你不必总是写诸如`impl<'a> Adventurer<'a>`这样的东西，因为结构已经显示了生命期。

在Rust中，生命期是很困难的，但这里有一些技巧可以避免对它们太过紧张。

- 你可以继续使用自有类型，使用克隆等，如果你想暂时避免它们。
- 很多时候，当编译器想要lifetime的时候，你只要在这里和那里写上<'a>就可以了。这只是一种 "别担心，我不会给你任何不够长寿的东西"的说法。
- 你可以每次只探索一下生命期。写一些拥有值的代码，然后把一个代码变成一个引用。编译器会开始抱怨，但也会给出一些建议。如果它变得太复杂，你可以撤销它，下次再试。

让我们用我们的代码来做这个，看看编译器怎么说。首先我们回去把生命期拿出来，同时实现`Display`。`Display`就打印`Adventurer`的名字。

```rust
// ⚠️
struct Adventurer {
    name: &str,
    hit_points: u32,
}

impl Adventurer {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

impl std::fmt::Display for Adventurer {
        fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
            write!(f, "{} has {} hit points.", self.name, self.hit_points)
        }
}

fn main() {}
```

第一个抱怨就是这个:

```text
error[E0106]: missing lifetime specifier
 --> src\main.rs:2:11
  |
2 |     name: &str,
  |           ^ expected named lifetime parameter
  |
help: consider introducing a named lifetime parameter
  |
1 | struct Adventurer<'a> {
2 |     name: &'a str,
  |
```

它建议怎么做:在Adventurer后面加上`<'a>`，以及`&'a str`。所以我们就这么做。

```rust
// ⚠️
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

impl std::fmt::Display for Adventurer {
        fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
            write!(f, "{} has {} hit points.", self.name, self.hit_points)
        }
}

fn main() {}
```

现在它对这些部分很满意，但对`impl`块感到奇怪。它希望我们提到它在使用引用。

```text
error[E0726]: implicit elided lifetime not allowed here
 --> src\main.rs:6:6
  |
6 | impl Adventurer {
  |      ^^^^^^^^^^- help: indicate the anonymous lifetime: `<'_>`

error[E0726]: implicit elided lifetime not allowed here
  --> src\main.rs:12:28
   |
12 | impl std::fmt::Display for Adventurer {
   |                            ^^^^^^^^^^- help: indicate the anonymous lifetime: `<'_>`
```

好了，我们将这些写进去......现在它工作了！现在我们可以创建一个`Adventurer`，然后用它做一些事情:

```rust
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer<'_> {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

impl std::fmt::Display for Adventurer<'_> {

        fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
            write!(f, "{} has {} hit points.", self.name, self.hit_points)
        }
}

fn main() {
    let mut billy = Adventurer {
        name: "Billy",
        hit_points: 100_000,
    };
    println!("{}", billy);
    billy.take_damage();
}
```

这个将打印:

```text
Billy has 100000 hit points.
Billy has 99980 hit points left!
```

所以你可以看到，lifetimes往往只是编译器想要确定。而且它通常很聪明，几乎可以猜到你想要的生命期，只需要你告诉它，它就可以确定了。

## 内部可变性

### Cell

**内部可变性**的意思是在内部有一点可变性。还记得在Rust中，你需要用`mut`来改变一个变量吗？也有一些方法可以不用`mut`这个词来改变它们。这是因为Rust有一些方法可以让你安全地在一个不可变的结构里面改变值。每一种方法都遵循一些规则，确保改变值仍然是安全的。

首先，让我们看一个简单的例子，我们会想要这样做:想象一下，一个叫`PhoneModel`的结构体有很多字段:

```rust
struct PhoneModel {
    company_name: String,
    model_name: String,
    screen_size: f32,
    memory: usize,
    date_issued: u32,
    on_sale: bool,
}

fn main() {
    let super_phone_3000 = PhoneModel {
        company_name: "YY Electronics".to_string(),
        model_name: "Super Phone 3000".to_string(),
        screen_size: 7.5,
        memory: 4_000_000,
        date_issued: 2020,
        on_sale: true,
    };

}
```

`PhoneModel`中的字段最好是不可变的，因为我们不希望数据改变。比如说`date_issued`和`screen_size`永远不会变。

但是里面有一个字段叫`on_sale`。一个手机型号先是会有销售(`true`)，但是后来公司会停止销售。我们能不能只让这一个字段可变？因为我们不想写`let mut super_phone_3000`。如果我们这样做，那么每个字段都会变得可变。

Rust有很多方法可以让一些不可变的东西里面有一些安全的可变性，最简单的方法叫做`Cell`。首先我们使用`use std::cell::Cell`，这样我们就可以每次只写`Cell`而不是`std::cell::Cell`。

然后我们把`on_sale: bool`改成`on_sale: Cell<bool>`。现在它不是一个bool:它是一个`Cell`，容纳了一个`bool`。

`Cell`有一个叫做`.set()`的方法，在这里你可以改变值。我们用`.set()`把`on_sale: true`改为`on_sale: Cell::new(true)`。

```rust
use std::cell::Cell;

struct PhoneModel {
    company_name: String,
    model_name: String,
    screen_size: f32,
    memory: usize,
    date_issued: u32,
    on_sale: Cell<bool>,
}

fn main() {
    let super_phone_3000 = PhoneModel {
        company_name: "YY Electronics".to_string(),
        model_name: "Super Phone 3000".to_string(),
        screen_size: 7.5,
        memory: 4_000_000,
        date_issued: 2020,
        on_sale: Cell::new(true),
    };

    // 10 years later, super_phone_3000 is not on sale anymore
    super_phone_3000.on_sale.set(false);
}
```

`Cell` 适用于所有类型，但对简单的 Copy 类型效果最好，因为它给出的是值，而不是引用。`Cell`有一个叫做`get()`的方法，它只对Copy类型有效。

另一个可以使用的类型是 `RefCell`。

### RefCell

`RefCell`是另一种无需声明`mut`而改变值的方法。它的意思是 "引用单元格"，就像 `Cell`，但使用引用而不是副本。

我们将创建一个 `User` 结构。到目前为止，你可以看到它与 `Cell` 类似。

```rust
use std::cell::RefCell;

#[derive(Debug)]
struct User {
    id: u32,
    year_registered: u32,
    username: String,
    active: RefCell<bool>,
    // Many other fields
}

fn main() {
    let user_1 = User {
        id: 1,
        year_registered: 2020,
        username: "User 1".to_string(),
        active: RefCell::new(true),
    };

    println!("{:?}", user_1.active);
}
```

这样就可以打印出`RefCell { value: true }`。

`RefCell`的方法有很多。其中两种是`.borrow()`和`.borrow_mut()`。使用这些方法，你可以做与`&`和`&mut`相同的事情。规则都是一样的:

- 多个不可变借用可以
- 一个可变的借用可以
- 但可变和不可变借用在一起是不行的

所以改变`RefCell`中的值是非常容易的。

```rust
// 🚧
user_1.active.replace(false);
println!("{:?}", user_1.active);
```

而且还有很多其他的方法，比如`replace_with`使用的是闭包。

```rust
// 🚧
let date = 2020;

user_1
    .active
    .replace_with(|_| if date < 2000 { true } else { false });
println!("{:?}", user_1.active);
```


但是你要小心使用`RefCell`，因为它是在运行时而不是编译时检查借用。运行时是指程序实际运行的时候(编译后)。所以这将会被编译，即使它是错误的。

```rust
use std::cell::RefCell;

#[derive(Debug)]
struct User {
    id: u32,
    year_registered: u32,
    username: String,
    active: RefCell<bool>,
    // Many other fields
}

fn main() {
    let user_1 = User {
        id: 1,
        year_registered: 2020,
        username: "User 1".to_string(),
        active: RefCell::new(true),
    };

    let borrow_one = user_1.active.borrow_mut(); // first mutable borrow - okay
    let borrow_two = user_1.active.borrow_mut(); // second mutable borrow - not okay
}
```

但如果你运行它，它就会立即崩溃。

```text
thread 'main' panicked at 'already borrowed: BorrowMutError', C:\Users\mithr\.rustup\toolchains\stable-x86_64-pc-windows-msvc\lib/rustlib/src/rust\src\libcore\cell.rs:877:9
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
error: process didn't exit successfully: `target\debug\rust_book.exe` (exit code: 101)
```

`already borrowed: BorrowMutError`是重要的部分。所以当你使用`RefCell`时，好编译**并**运行检查。

### Mutex

`Mutex`是另一种改变数值的方法，不需要声明`mut`。Mutex的意思是`mutual exclusion`，也就是 "一次只能改一个"。这就是为什么`Mutex`是安全的，因为它每次只让一个进程改变它。为了做到这一点，它使用了`.lock()`。`Lock`就像从里面锁上一扇门。你进入一个房间，锁上门，现在你可以在房间里面改变东西。别人不能进来阻止你，因为你把门锁上了。

`Mutex`通过例子更容易理解:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5); // A new Mutex<i32>. We don't need to say mut
    let mut mutex_changer = my_mutex.lock().unwrap(); // mutex_changer is a MutexGuard
                                                     // It has to be mut because we will change it
                                                     // Now it has access to the Mutex
                                                     // Let's print my_mutex to see:

    println!("{:?}", my_mutex); // This prints "Mutex { data: <locked> }"
                                // So we can't access the data with my_mutex now,
                                // only with mutex_changer

    println!("{:?}", mutex_changer); // This prints 5. Let's change it to 6.

    *mutex_changer = 6; // mutex_changer is a MutexGuard<i32> so we use * to change the i32

    println!("{:?}", mutex_changer); // Now it says 6
}
```

但是`mutex_changer`做完后还是有锁。我们该如何阻止它呢？`Mutex`在`MutexGuard`超出范围时就会被解锁。"超出范围"表示该代码块已经完成。比如说:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    {
        let mut mutex_changer = my_mutex.lock().unwrap();
        *mutex_changer = 6;
    } // mutex_changer goes out of scope - now it is gone. It is not locked anymore

    println!("{:?}", my_mutex); // Now it says: Mutex { data: 6 }
}
```

如果你不想使用不同的`{}`代码块，你可以使用`std::mem::drop(mutex_changer)`。`std::mem::drop`的意思是 "让这个超出范围"。

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    let mut mutex_changer = my_mutex.lock().unwrap();
    *mutex_changer = 6;
    std::mem::drop(mutex_changer); // drop mutex_changer - it is gone now
                                   // and my_mutex is unlocked

    println!("{:?}", my_mutex); // Now it says: Mutex { data: 6 }
}
```

你必须小心使用 `Mutex`，因为如果另一个变量试图 `lock`它，它会等待。

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    let mut mutex_changer = my_mutex.lock().unwrap(); // mutex_changer has the lock
    let mut other_mutex_changer = my_mutex.lock().unwrap(); // other_mutex_changer wants the lock
                                                            // the program is waiting
                                                            // and waiting
                                                            // and will wait forever.

    println!("This will never print...");
}
```

还有一种方法是`try_lock()`。然后它会试一次，如果没能锁上就会放弃。`try_lock().unwrap()`就不要做了，因为如果不成功它就会崩溃。`if let`或`match`比较好。

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    let mut mutex_changer = my_mutex.lock().unwrap();
    let mut other_mutex_changer = my_mutex.try_lock(); // try to get the lock

    if let Ok(value) = other_mutex_changer {
        println!("The MutexGuard has: {}", value)
    } else {
        println!("Didn't get the lock")
    }
}
```

另外，你不需要创建一个变量来改变`Mutex`。你可以直接这样做:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);

    *my_mutex.lock().unwrap() = 6;

    println!("{:?}", my_mutex);
}
```

`*my_mutex.lock().unwrap() = 6;`的意思是 "解锁my_mutex并使其成为6"。没有任何变量来保存它，所以你不需要调用 `std::mem::drop`。如果你愿意，你可以做100次--这并不重要。

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);

    for _ in 0..100 {
        *my_mutex.lock().unwrap() += 1; // locks and unlocks 100 times
    }

    println!("{:?}", my_mutex);
}
```

### RwLock

`RwLock`的意思是 "读写锁"。它像`Mutex`，但也像`RefCell`。你用`.write().unwrap()`代替`.lock().unwrap()`来改变它。但你也可以用`.read().unwrap()`来获得读权限。它和`RefCell`一样，遵循这些规则:

- 很多`.read()`变量可以
- 一个`.write()`变量可以
- 但多个`.write()`或`.read()`与`.write()`一起是不行的

如果在无法访问的情况下尝试`.write()`，程序将永远运行。

```rust
use std::sync::RwLock;

fn main() {
    let my_rwlock = RwLock::new(5);

    let read1 = my_rwlock.read().unwrap(); // one .read() is fine
    let read2 = my_rwlock.read().unwrap(); // two .read()s is also fine

    println!("{:?}, {:?}", read1, read2);

    let write1 = my_rwlock.write().unwrap(); // uh oh, now the program will wait forever
}
```

所以我们用`std::mem::drop`，就像用`Mutex`一样。

```rust
use std::sync::RwLock;
use std::mem::drop; // We will use drop() many times

fn main() {
    let my_rwlock = RwLock::new(5);

    let read1 = my_rwlock.read().unwrap();
    let read2 = my_rwlock.read().unwrap();

    println!("{:?}, {:?}", read1, read2);

    drop(read1);
    drop(read2); // we dropped both, so we can use .write() now

    let mut write1 = my_rwlock.write().unwrap();
    *write1 = 6;
    drop(write1);
    println!("{:?}", my_rwlock);
}
```

而且你也可以使用`try_read()`和`try_write()`。

```rust
use std::sync::RwLock;

fn main() {
    let my_rwlock = RwLock::new(5);

    let read1 = my_rwlock.read().unwrap();
    let read2 = my_rwlock.read().unwrap();

    if let Ok(mut number) = my_rwlock.try_write() {
        *number += 10;
        println!("Now the number is {}", number);
    } else {
        println!("Couldn't get write access, sorry!")
    };
}
```

## Cow

Cow是一个非常方便的枚举。它的意思是 "写时克隆"，如果你不需要`String`，可以返回一个`&str`，如果你需要，可以返回一个`String`。(它也可以对数组与Vec等做同样的处理)。

为了理解它，我们看一下签名。它说

```rust
pub enum Cow<'a, B>
where
    B: 'a + ToOwned + ?Sized,
 {
    Borrowed(&'a B),
    Owned(<B as ToOwned>::Owned),
}

fn main() {}
```

你马上就知道，`'a`意味着它可以和引用一起工作。`ToOwned`的特性意味着它是一个可以变成拥有类型的类型。例如，`str`通常是一个引用(`&str`)，你可以把它变成一个拥有的`String`。

接下来是`?Sized`。这意味着 "也许是Sized，但也许不是"。Rust中几乎每个类型都是Sized的，但像`str`这样的类型却不是。这就是为什么我们需要一个 `&` 来代替 `str`，因为编译器不知道大小。所以，如果你想要一个可以使用 `str` 这样的trait，你可以添加 `?Sized.`

接下来是`enum`的变种。它们是 `Borrowed` 和 `Owned`。

想象一下，你有一个返回 `Cow<'static, str>` 的函数。如果你告诉函数返回`"My message".into()`，它就会查看类型:"My message"是`str`. 这是一个`Borrowed`的类型，所以它选择`Borrowed(&'a B)`。所以它就变成了`Cow::Borrowed(&'static str)`。

而如果你给它一个`format!("{}", "My message").into()`，那么它就会查看类型。这次是一个`String`，因为`format!`创建了`String`。所以这次会选择 "Owned"。

下面是一个测试`Cow`的例子。我们将把一个数字放入一个函数中，返回一个`Cow<'static, str>`。根据这个数字，它会创建一个`&str`或`String`。然后它使用`.into()`将其变成`Cow`。这样做的时候，它就会选择`Cow::Borrowed`或者`Cow::Owned`。那我们就匹配一下，看看它选的是哪一个。

```rust
use std::borrow::Cow;

fn modulo_3(input: u8) -> Cow<'static, str> {
    match input % 3 {
        0 => "Remainder is 0".into(),
        1 => "Remainder is 1".into(),
        remainder => format!("Remainder is {}", remainder).into(),
    }
}

fn main() {
    for number in 1..=6 {
        match modulo_3(number) {
            Cow::Borrowed(message) => println!("{} went in. The Cow is borrowed with this message: {}", number, message),
            Cow::Owned(message) => println!("{} went in. The Cow is owned with this message: {}", number, message),
        }
    }
}
```

这个打印:

```text
1 went in. The Cow is borrowed with this message: Remainder is 1
2 went in. The Cow is owned with this message: Remainder is 2
3 went in. The Cow is borrowed with this message: Remainder is 0
4 went in. The Cow is borrowed with this message: Remainder is 1
5 went in. The Cow is owned with this message: Remainder is 2
6 went in. The Cow is borrowed with this message: Remainder is 0
```

`Cow`还有一些其他的方法，比如`into_owned` 或者 `into_borrowed`，这样如果你需要的话，你可以改变它。

## 类型别名

类型别名的意思是 "给某个类型一个新的名字"。类型别名非常简单。通常，当您有一个很长的类型，而又不想每次都写它时，您就会使用它们。当您想给一个类型起一个更好的名字，便于记忆时，也可以使用它。下面是两个类型别名的例子。

这里是一个不难的类型，但是你想让你的代码更容易被其他人(或者你)理解。

```rust
type CharacterVec = Vec<char>;

fn main() {}
```


这是一种非常难读的类型:

```rust
// this return type is extremely long
fn returns<'a>(input: &'a Vec<char>) -> std::iter::Take<std::iter::Skip<std::slice::Iter<'a, char>>> {
    input.iter().skip(4).take(5)
}

fn main() {}
```

所以你可以改成这样。

```rust
type SkipFourTakeFive<'a> = std::iter::Take<std::iter::Skip<std::slice::Iter<'a, char>>>;

fn returns<'a>(input: &'a Vec<char>) -> SkipFourTakeFive {
    input.iter().skip(4).take(5)
}

fn main() {}
```

当然，你也可以导入元素，让类型更短:

```rust
use std::iter::{Take, Skip};
use std::slice::Iter;

fn returns<'a>(input: &'a Vec<char>) -> Take<Skip<Iter<'a, char>>> {
    input.iter().skip(4).take(5)
}

fn main() {}
```

所以你可以根据自己的喜好来决定在你的代码中什么是最好看的。

请注意，这并没有创建一个实际的新类型。它只是一个代替现有类型的名称。所以如果你写了 `type File = String;`，编译器只会看到 `String`。所以这将打印出 `true`。

```rust
type File = String;

fn main() {
    let my_file = File::from("I am file contents");
    let my_string = String::from("I am file contents");
    println!("{}", my_file == my_string);
}
```

那么如果你想要一个实际的新类型呢？

如果你想要一个新的文件类型，而编译器看到的是`File`，你可以把它放在一个结构中。

```rust
struct File(String); // File is a wrapper around String

fn main() {
    let my_file = File(String::from("I am file contents"));
    let my_string = String::from("I am file contents");
}
```

现在这样就不行了，因为它们是两种不同的类型。

```rust
struct File(String); // File is a wrapper around String

fn main() {
    let my_file = File(String::from("I am file contents"));
    let my_string = String::from("I am file contents");
    println!("{}", my_file == my_string);  // ⚠️ cannot compare File with String
}
```

如果你想比较里面的String，可以用my_file.0:

```rust
struct File(String);

fn main() {
    let my_file = File(String::from("I am file contents"));
    let my_string = String::from("I am file contents");
    println!("{}", my_file.0 == my_string); // my_file.0 is a String, so this prints true
}
```

### 在函数中导入和重命名

通常你会在程序的顶部写上`use`，像这样。

```rust
use std::cell::{Cell, RefCell};

fn main() {}
```

但我们看到，你可以在任何地方这样做，特别是在函数中使用名称较长的enum。下面是一个例子:

```rust
enum MapDirection {
    North,
    NorthEast,
    East,
    SouthEast,
    South,
    SouthWest,
    West,
    NorthWest,
}

fn main() {}

fn give_direction(direction: &MapDirection) {
    match direction {
        MapDirection::North => println!("You are heading north."),
        MapDirection::NorthEast => println!("You are heading northeast."),
        // So much more left to type...
        // ⚠️ because we didn't write every possible variant
    }
}
```

所以现在我们要在函数里面导入MapDirection。也就是说，在函数里面你可以直接写`North`等。

```rust
enum MapDirection {
    North,
    NorthEast,
    East,
    SouthEast,
    South,
    SouthWest,
    West,
    NorthWest,
}

fn main() {}

fn give_direction(direction: &MapDirection) {
    use MapDirection::*; // Import everything in MapDirection
    let m = "You are heading";

    match direction {
        North => println!("{} north.", m),
        NorthEast => println!("{} northeast.", m),
        // This is a bit better
        // ⚠️
    }
}
```

我们已经看到`::*`的意思是 "导入::之后的所有内容"。在我们的例子中，这意味着`North`，`NorthEast`......一直到`NorthWest`。当你导入别人的代码时，你也可以这样做，但如果代码非常大，你可能会有问题。如果它有一些元素和你的代码是一样的呢？所以一般情况下最好不要一直使用`::*`，除非你有把握。很多时候你在别人的代码里看到一个叫`prelude`的部分，里面有你可能需要的所有主要元素。那么你通常会这样使用:`name::prelude::*`。 我们将在 `modules` 和 `crates` 的章节中更多地讨论这个问题。

您也可以使用 `as` 来更改名称。例如，也许你正在使用别人的代码，而你不能改变枚举中的名称。

```rust
enum FileState {
    CannotAccessFile,
    FileOpenedAndReady,
    NoSuchFileExists,
    SimilarFileNameInNextDirectory,
}

fn main() {}
```

那么你就可以
1) 导入所有的东西
2) 更改名称

```rust
enum FileState {
    CannotAccessFile,
    FileOpenedAndReady,
    NoSuchFileExists,
    SimilarFileNameInNextDirectory,
}

fn give_filestate(input: &FileState) {
    use FileState::{
        CannotAccessFile as NoAccess,
        FileOpenedAndReady as Good,
        NoSuchFileExists as NoFile,
        SimilarFileNameInNextDirectory as OtherDirectory
    };
    match input {
        NoAccess => println!("Can't access file."),
        Good => println!("Here is your file"),
        NoFile => println!("Sorry, there is no file by that name."),
        OtherDirectory => println!("Please check the other directory."),
    }
}

fn main() {}
```

所以现在你可以写`OtherDirectory`而不是`FileState::SimilarFileNameInNextDirectory`。

## todo!宏

有时你想粗略写点写代码帮助你想象你的项目。例如，想象一个简单的项目，用书籍做一些事情。下面是你写的时候的想法:

```rust
struct Book {} // Okay, first I need a book struct.
               // Nothing in there yet - will add later

enum BookType { // A book can be hardcover or softcover, so add an enum
    HardCover,
    SoftCover,
}

fn get_book(book: &Book) -> Option<String> {} // ⚠️ get_book should take a &Book and return an Option<String>

fn delete_book(book: Book) -> Result<(), String> {} // delete_book should take a Book and return a Result...
                                                    // TODO: impl block and make these functions methods...
fn check_book_type(book_type: &BookType) { // Let's make sure the match statement works
    match book_type {
        BookType::HardCover => println!("It's hardcover"),
        BookType::SoftCover => println!("It's softcover"),
    }
}

fn main() {
    let book_type = BookType::HardCover;
    check_book_type(&book_type); // Okay, let's check this function!
}
```

但Rust对`get_book`和`delete_book`不满意。它说

```text
error[E0308]: mismatched types
  --> src\main.rs:32:29
   |
32 | fn get_book(book: &Book) -> Option<String> {}
   |    --------                 ^^^^^^^^^^^^^^ expected enum `std::option::Option`, found `()`
   |    |
   |    implicitly returns `()` as its body has no tail or `return` expression
   |
   = note:   expected enum `std::option::Option<std::string::String>`
           found unit type `()`

error[E0308]: mismatched types
  --> src\main.rs:34:31
   |
34 | fn delete_book(book: Book) -> Result<(), String> {}
   |    -----------                ^^^^^^^^^^^^^^^^^^ expected enum `std::result::Result`, found `()`
   |    |
   |    implicitly returns `()` as its body has no tail or `return` expression
   |
   = note:   expected enum `std::result::Result<(), std::string::String>`
           found unit type `()`
```

但是你现在不关心`get_book`和`delete_book`。这时你可以使用`todo!()`。如果你把这个加到函数中，Rust不会抱怨，而且会编译。

```rust
struct Book {}

fn get_book(book: &Book) -> Option<String> {
    todo!() // todo means "I will do it later, please be quiet"
}

fn delete_book(book: Book) -> Result<(), String> {
    todo!()
}

fn main() {}
```

所以现在代码编译，你可以看到`check_book_type`的结果:`It's hardcover`。

但是要小心，因为它只是编译--你不能使用函数。如果你调用里面有`todo!()`的函数，它就会崩溃。

另外，`todo!()`函数仍然需要真实的输入和输出类型。如果你只写这个，它将无法编译。

```rust
struct Book {}

fn get_book(book: &Book) -> WorldsBestType { // ⚠️
    todo!()
}

fn main() {}
```

它会说

```text
error[E0412]: cannot find type `WorldsBestType` in this scope
  --> src\main.rs:32:29
   |
32 | fn get_book(book: &Book) -> WorldsBestType {
   |                             ^^^^^^^^^^^^^^ not found in this scope
```

`todo!()`其实和另一个宏一样：`unimplemented!()`。程序员们经常使用 `unimplemented!()`，但打字时太长了，所以他们创建了 `todo!()`，它比较短。

## Rc

Rc的意思是 "reference counter"(引用计数器)。你知道在Rust中，每个变量只能有一个所有者。这就是为什么这个不能工作的原因:

```rust
fn takes_a_string(input: String) {
    println!("It is: {}", input)
}

fn also_takes_a_string(input: String) {
    println!("It is: {}", input)
}

fn main() {
    let user_name = String::from("User MacUserson");

    takes_a_string(user_name);
    also_takes_a_string(user_name); // ⚠️
}
```

`takes_a_string`取了`user_name`之后，你就不能再使用了。这里没有问题:你可以直接给它`user_name.clone()`。但有时一个变量是一个结构的一部分，也许你不能克隆这个结构；或者`String`真的很长，你不想克隆它。这些都是`Rc`的一些原因，它让你拥有多个所有者。`Rc`就像一个优秀的办公人员。`Rc`写下谁拥有所有权，以及有多少个。然后一旦所有者的数量下降到0，这个变量就可以消失了。

下面是如何使用`Rc`。首先想象两个结构:一个叫 `City`，另一个叫 `CityData`。`City`有一个城市的信息，而`CityData`把所有的城市都放在`Vec`中。

```rust
#[derive(Debug)]
struct City {
    name: String,
    population: u32,
    city_history: String,
}

#[derive(Debug)]
struct CityData {
    names: Vec<String>,
    histories: Vec<String>,
}

fn main() {
    let calgary = City {
        name: "Calgary".to_string(),
        population: 1_200_000,
           // Pretend that this string is very very long
        city_history: "Calgary began as a fort called Fort Calgary that...".to_string(),
    };

    let canada_cities = CityData {
        names: vec![calgary.name], // This is using calgary.name, which is short
        histories: vec![calgary.city_history], // But this String is very long
    };

    println!("Calgary's history is: {}", calgary.city_history);  // ⚠️
}
```

当然，这是不可能的，因为`canada_cities`现在拥有数据，而`calgary`没有。它说:

```text
error[E0382]: borrow of moved value: `calgary.city_history`
  --> src\main.rs:27:42
   |
24 |         histories: vec![calgary.city_history], // But this String is very long
   |                         -------------------- value moved here
...
27 |     println!("Calgary's history is: {}", calgary.city_history);  // ⚠️
   |                                          ^^^^^^^^^^^^^^^^^^^^ value borrowed here after move
   |
   = note: move occurs because `calgary.city_history` has type `std::string::String`, which does not implement the `Copy` trait
```

我们可以克隆名称:`names: vec![calgary.name.clone()]`，但是我们不想克隆`city_history`，因为它很长。所以我们可以用一个`Rc`。

增加`use`的声明。

```rust
use std::rc::Rc;

fn main() {}
```

然后用`Rc`把`String`包围起来:

```rust
use std::rc::Rc;

#[derive(Debug)]
struct City {
    name: String,
    population: u32,
    city_history: Rc<String>,
}

#[derive(Debug)]
struct CityData {
    names: Vec<String>,
    histories: Vec<Rc<String>>,
}

fn main() {}
```

要添加一个新的引用，你必须`clone` `Rc`。但是等一下，我们不是想避免使用`.clone()`吗？不完全是:我们不想克隆整个String。但是一个`Rc`的克隆只是克隆了指针--它基本上是没有开销的。这就像在一盒书上贴上一个名字贴纸，以表明有两个人拥有它，而不是做一盒全新的书。

你可以用`item.clone()`或者用`Rc::clone(&item)`来克隆一个叫`item`的`Rc`。所以calgary.city_history有两个所有者。
 我们可以用`Rc::strong_count(&item)`查询拥有者数量。另外我们再增加一个新的所有者。现在我们的代码是这样的:

```rust
use std::rc::Rc;

#[derive(Debug)]
struct City {
    name: String,
    population: u32,
    city_history: Rc<String>, // String inside an Rc
}

#[derive(Debug)]
struct CityData {
    names: Vec<String>,
    histories: Vec<Rc<String>>, // A Vec of Strings inside Rcs
}

fn main() {
    let calgary = City {
        name: "Calgary".to_string(),
        population: 1_200_000,
           // Pretend that this string is very very long
        city_history: Rc::new("Calgary began as a fort called Fort Calgary that...".to_string()), // Rc::new() to make the Rc
    };

    let canada_cities = CityData {
        names: vec![calgary.name],
        histories: vec![calgary.city_history.clone()], // .clone() to increase the count
    };

    println!("Calgary's history is: {}", calgary.city_history);
    println!("{}", Rc::strong_count(&calgary.city_history));
    let new_owner = calgary.city_history.clone();
}
```

这就打印出了`2`。而`new_owner`现在是`Rc<String>`。现在如果我们用`println!("{}", Rc::strong_count(&calgary.city_history));`，我们得到`3`。

那么，如果有强指针，是否有弱指针呢？是的，有。弱指针是有用的，因为如果两个`Rc`互相指向对方，它们就不会死。这就是所谓的 "引用循环"。如果第1项对第2项有一个Rc，而第2项对第1项有一个Rc，它们不能到0，在这种情况下，要使用弱引用。那么`Rc`就会对引用进行计数，但如果只有弱引用，那么它就会死掉。你使用`Rc::downgrade(&item)`而不是`Rc::clone(&item)`来创建弱引用。另外，需要用`Rc::weak_count(&item)`来查看弱引用数。

## 多线程

如果你使用多个线程，你可以同时做很多事情。现代计算机有一个以上的核心，所以它们可以同时做多件事情，Rust让你使用它们。Rust使用的线程被称为 "OS线程"。OS线程意味着操作系统在不同的核上创建线程。(其他一些语言使用 "green threads"，功能较少)


你用`std::thread::spawn`创建线程，然后用一个闭包来告诉它该怎么做。线程很有趣，因为它们同时运行，你可以测试它，看看会发生什么。下面是一个简单的例子。

```rust
fn main() {
    std::thread::spawn(|| {
        println!("I am printing something");
    });
}
```

如果你运行这个，每次都会不一样。有时会打印，有时不会打印(这也取决于你的电脑速度)。这是因为有时`main()`在线程完成之前就完成了。而当`main()`完成后，程序就结束了。这在`for`循环中更容易看到。

```rust
fn main() {
    for _ in 0..10 { // set up ten threads
        std::thread::spawn(|| {
            println!("I am printing something");
        });
    }   // Now the threads start.
}       // How many can finish before main() ends here?
```

通常在`main`结束之前，大约会打印出四条线程，但总是不一样。如果你的电脑速度比较快，那么可能就不会打印了。另外，有时线程会崩溃。

```text
thread 'thread 'I am printing something
thread '<unnamed><unnamed>thread '' panicked at '<unnamed>I am printing something
' panicked at 'thread '<unnamed>cannot access stdout during shutdown' panicked at '<unnamed>thread 'cannot access stdout during
shutdown
```

这是在程序关闭时，线程试图做一些正确的事情时出现的错误。

你可以给电脑做一些事情，这样它就不会马上关闭了。

```rust
fn main() {
    for _ in 0..10 {
        std::thread::spawn(|| {
            println!("I am printing something");
        });
    }
    for _ in 0..1_000_000 { // make the program declare "let x = 9" one million times
                            // It has to finish this before it can exit the main function
        let _x = 9;
    }
}
```

但这是一个让线程有时间完成的愚蠢方法。更好的方法是将线程绑定到一个变量上。如果你加上 `let`，你就能创建一个 `JoinHandle`。你可以在`spawn`的签名中看到这一点:

```text
pub fn spawn<F, T>(f: F) -> JoinHandle<T>
where
    F: FnOnce() -> T,
    F: Send + 'static,
    T: Send + 'static,
```

(`f`是闭包--我们将在后面学习如何将闭包放入我们的函数中)

所以现在我们每次都有`JoinHandle`。

```rust
fn main() {
    for _ in 0..10 {
        let handle = std::thread::spawn(|| {
            println!("I am printing something");
        });

    }
}
```

`handle`现在是`JoinHandle`。我们怎么处理它呢？我们使用一个叫做 `.join()` 的方法。这个方法的意思是 "等待所有线程完成"(它等待线程加入它)。所以现在只要写`handle.join()`，它就会等待每个线程完成。

```rust
fn main() {
    for _ in 0..10 {
        let handle = std::thread::spawn(|| {
            println!("I am printing something");
        });

        handle.join(); // Wait for the threads to finish
    }
}
```

现在我们就来了解一下三种类型的闭包。这三种类型是

- `FnOnce`: 取整个值
- `FnMut`: 取一个可变引用
- `Fn`: 取一个普通引用

如果可以的话，闭包会尽量使用`Fn`。但如果它需要改变值，它将使用 `FnMut`，而如果它需要取整个值，它将使用 `FnOnce`。`FnOnce`是个好名字，因为它解释了它的作用:它取一次值，然后就不能再取了。

下面是一个例子。

```rust
fn main() {
    let my_string = String::from("I will go into the closure");
    let my_closure = || println!("{}", my_string);
    my_closure();
    my_closure();
}
```

`String`没有实现`Copy`，所以`my_closure()`是`Fn`: 它拿到一个引用

如果我们改变`my_string`，它变成`FnMut`。

```rust
fn main() {
    let mut my_string = String::from("I will go into the closure");
    let mut my_closure = || {
        my_string.push_str(" now");
        println!("{}", my_string);
    };
    my_closure();
    my_closure();
}
```

这个打印:

```text
I will go into the closure now
I will go into the closure now now
```

而如果按值获取，则是`FnOnce`。

```rust
fn main() {
    let my_vec: Vec<i32> = vec![8, 9, 10];
    let my_closure = || {
        my_vec
            .into_iter() // into_iter takes ownership
            .map(|x| x as u8) // turn it into u8
            .map(|x| x * 2) // multiply by 2
            .collect::<Vec<u8>>() // collect into a Vec
    };
    let new_vec = my_closure();
    println!("{:?}", new_vec);
}
```

我们是按值取的，所以我们不能多跑`my_closure()`次。这就是名字的由来。

那么现在回到线程。让我们试着从外部引入一个值:

```rust
fn main() {
    let mut my_string = String::from("Can I go inside the thread?");

    let handle = std::thread::spawn(|| {
        println!("{}", my_string); // ⚠️
    });

    handle.join();
}
```

编译器说这个不行。

```text
error[E0373]: closure may outlive the current function, but it borrows `my_string`, which is owned by the current function
  --> src\main.rs:28:37
   |
28 |     let handle = std::thread::spawn(|| {
   |                                     ^^ may outlive borrowed value `my_string`
29 |         println!("{}", my_string);
   |                        --------- `my_string` is borrowed here
   |
note: function requires argument type to outlive `'static`
  --> src\main.rs:28:18
   |
28 |       let handle = std::thread::spawn(|| {
   |  __________________^
29 | |         println!("{}", my_string);
30 | |     });
   | |______^
help: to force the closure to take ownership of `my_string` (and any other referenced variables), use the `move` keyword
   |
28 |     let handle = std::thread::spawn(move || {
   |                                     ^^^^^^^
```

这条信息很长，但很有用:它说到``use the `move` keyword``。问题是我们可以在线程使用`my_string`时对它做任何事情，但线程并不拥有它。这将是不安全的。

让我们试试其他行不通的东西。

```rust
fn main() {
    let mut my_string = String::from("Can I go inside the thread?");

    let handle = std::thread::spawn(|| {
        println!("{}", my_string); // now my_string is being used as a reference
    });

    std::mem::drop(my_string);  // ⚠️ We try to drop it here. But the thread still needs it.

    handle.join();
}
```

所以你要用`move`来取值，现在安全了:

```rust
fn main() {
    let mut my_string = String::from("Can I go inside the thread?");

    let handle = std::thread::spawn(move|| {
        println!("{}", my_string);
    });

    std::mem::drop(my_string);  // ⚠️ we can't drop, because handle has it. So this won't work

    handle.join();
}
```

所以我们把`std::mem::drop`删掉，现在就可以了。`handle`取`my_string`，我们的代码就安全了。

```rust
fn main() {
    let mut my_string = String::from("Can I go inside the thread?");

    let handle = std::thread::spawn(move|| {
        println!("{}", my_string);
    });

    handle.join();
}
```

所以只要记住:如果你在线程中需要一个来自线程外的值，你需要使用`move`。



## 函数中的闭包

闭包是伟大的。那么我们如何把它们放到自己的函数中呢？

你可以创建自己的函数来接受闭包，但是在函数里面就不那么自由了，你必须决定类型。在函数外部，一个闭包可以在`Fn`、`FnMut`和`FnOnce`之间自行决定，但在函数内部你必须选择一个。最好的理解方式是看几个函数签名。
 这里是`.all()`的那个。我们记得，它检查一个迭代器，看看所有的东西是否是`true`(取决于你决定是`true`还是`false`)。它的部分签名是这样说的。


```rust
    fn all<F>(&mut self, f: F) -> bool    // 🚧
    where
        F: FnMut(Self::Item) -> bool,
```

`fn all<F>`:这告诉你有一个通用类型`F`。一个闭包总是泛型，因为每次都是不同的类型。

`(&mut self, f: F)`:`&mut self`告诉你这是一个方法。`f: F`通常你看到的是一个闭包:这是变量名和类型。 当然，`f`和`F`并没有什么特别之处，它们可以是不同的名字。如果你愿意，你可以写`my_closure: Closure`--这并不重要。但在签名中，你几乎总是看到`f: F`。

接下来是关于闭包的部分:`F: FnMut(Self::Item) -> bool`。在这里，它决定了闭包是 `FnMut`，所以它可以改变值。它改变了`Self::Item`的值，这是它所取的迭代器。而且它必须返回 `true` 或 `false`。

这里是一个更简单的签名，有一个闭包。

```rust
fn do_something<F>(f: F)    // 🚧
where
    F: FnOnce(),
{
    f();
}
```

这只是说它接受一个闭包，取值(`FnOnce`=取值)，而不返回任何东西。所以现在我们可以调用这个什么都不取的闭包，做我们喜欢做的事情。我们将创建一个 `Vec`，然后对它进行迭代，只是为了展示我们现在可以做什么。

```rust
fn do_something<F>(f: F)
where
    F: FnOnce(),
{
    f();
}

fn main() {
    let some_vec = vec![9, 8, 10];
    do_something(|| {
        some_vec
            .into_iter()
            .for_each(|x| println!("The number is: {}", x));
    })
}
```

一个更真实的例子，我们将再次创建一个 `City` 结构体。这次 `City` 结构体有更多关于年份和人口的数据。它有一个 `Vec<u32>` 来表示所有的年份，还有一个 `Vec<u32>` 来表示所有的人口。

`City`有两个方法:`new()`用于创建一个新的`City`, `.city_data()`有个闭包参数。当我们使用 `.city_data()` 时，它给我们提供了年份和人口以及一个闭包，所以我们可以对数据做我们想做的事情。闭包类型是 `FnMut`，所以我们可以改变数据。它看起来像这样:

```rust
#[derive(Debug)]
struct City {
    name: String,
    years: Vec<u32>,
    populations: Vec<u32>,
}

impl City {
    fn new(name: &str, years: Vec<u32>, populations: Vec<u32>) -> Self {

        Self {
            name: name.to_string(),
            years,
            populations,
        }
    }

    fn city_data<F>(&mut self, mut f: F) // We bring in self, but only f is generic F. f is the closure

    where
        F: FnMut(&mut Vec<u32>, &mut Vec<u32>), // The closure takes mutable vectors of u32
                                                // which are the year and population data
    {
        f(&mut self.years, &mut self.populations) // Finally this is the actual function. It says
                                                  // "use a closure on self.years and self.populations"
                                                  // We can do whatever we want with the closure
    }
}

fn main() {
    let years = vec![
        1372, 1834, 1851, 1881, 1897, 1925, 1959, 1989, 2000, 2005, 2010, 2020,
    ];
    let populations = vec![
        3_250, 15_300, 24_000, 45_900, 58_800, 119_800, 283_071, 478_974, 400_378, 401_694,
        406_703, 437_619,
    ];
    // Now we can create our city
    let mut tallinn = City::new("Tallinn", years, populations);

    // Now we have a .city_data() method that has a closure. We can do anything we want.

    // First let's put the data for 5 years together and print it.
    tallinn.city_data(|city_years, city_populations| { // We can call the input anything we want
        let new_vec = city_years
            .into_iter()
            .zip(city_populations.into_iter()) // Zip the two together
            .take(5)                           // but only take the first 5
            .collect::<Vec<(_, _)>>(); // Tell Rust to decide the type inside the tuple
        println!("{:?}", new_vec);
    });

    // Now let's add some data for the year 2030
    tallinn.city_data(|x, y| { // This time we just call the input x and y
        x.push(2030);
        y.push(500_000);
    });

    // We don't want the 1834 data anymore
    tallinn.city_data(|x, y| {
        let position_option = x.iter().position(|x| *x == 1834);
        if let Some(position) = position_option {
            println!(
                "Going to delete {} at position {:?} now.",
                x[position], position
            ); // Confirm that we delete the right item
            x.remove(position);
            y.remove(position);
        }
    });

    println!(
        "Years left are {:?}\nPopulations left are {:?}",
        tallinn.years, tallinn.populations
    );
}
```

这将打印出我们调用`.city_data().`的所有时间的结果:

```text
[(1372, 3250), (1834, 15300), (1851, 24000), (1881, 45900), (1897, 58800)]
Going to delete 1834 at position 1 now.
Years left are [1372, 1851, 1881, 1897, 1925, 1959, 1989, 2000, 2005, 2010, 2020, 2030]
Populations left are [3250, 24000, 45900, 58800, 119800, 283071, 478974, 400378, 401694, 406703, 437619, 500000]
```


## impl Trait

`impl Trait`与泛型类似。你还记得，泛型使用一个类型 `T`(或任何其他名称)，然后在程序编译时决定。首先我们来看一个具体的类型:

```rust
fn gives_higher_i32(one: i32, two: i32) {
    let higher = if one > two { one } else { two };
    println!("{} is higher.", higher);
}

fn main() {
    gives_higher_i32(8, 10);
}
```

这个打印:`10 is higher.`.

但是这个只接受`i32`，所以现在我们要把它做成通用的。我们需要比较，我们需要用`{}`打印，所以我们的类型T需要`PartialOrd`和`Display`。记住，这意味着 "只接受已经实现`PartialOrd`和`Display`的类型"。

```rust
use std::fmt::Display;

fn gives_higher_i32<T: PartialOrd + Display>(one: T, two: T) {
    let higher = if one > two { one } else { two };
    println!("{} is higher.", higher);
}

fn main() {
    gives_higher_i32(8, 10);
}
```

现在我们来看看`impl Trait`，它也是类似的。我们可以引入一个类型 `impl Trait`，而不是 `T`。然后它将带入一个实现该特性的类型。这几乎是一样的。

```rust
fn prints_it(input: impl Into<String> + std::fmt::Display) { // Takes anything that can turn into a String and has Display
    println!("You can print many things, including {}", input);
}

fn main() {
    let name = "Tuon";
    let string_name = String::from("Tuon");
    prints_it(name);
    prints_it(string_name);
}
```

然而，更有趣的是，我们可以返回 `impl Trait`，这让我们可以返回闭包，因为它们的函数签名是trait。你可以在有它们的方法的签名中看到这一点。例如，这是 `.map()` 的签名。

```rust
fn map<B, F>(self, f: F) -> Map<Self, F>     // 🚧
    where
        Self: Sized,
        F: FnMut(Self::Item) -> B,
    {
        Map::new(self, f)
    }
```

`fn map<B, F>(self, f: F)`的意思是，它需要两个通用类型。`F`是指从实现`.map()`的容器中取一个元素的函数，`B`是该函数的返回类型。然后在`where`之后，我们看到的是trait bound。("trait bound"的意思是 "它必须有这个trait"。)一个是`Sized`，接下来是闭包签名。它必须是一个 `FnMut`，并在 `Self::Item` 上做闭包，也就是你给它的迭代器。然后它返回`B`。

所以我们可以用同样的方法来返回一个闭包。要返回一个闭包，使用 `impl`，然后是闭包签名。一旦你返回它，你就可以像使用一个函数一样使用它。下面是一个函数的小例子，它根据你输入的文本给出一个闭包。如果你输入 "double "或 "triple"，那么它就会把它乘以2或3，否则就会返给你相同的数字。因为它是一个闭包，我们可以做任何我们想做的事情，所以我们也打印一条信息。

```rust
fn returns_a_closure(input: &str) -> impl FnMut(i32) -> i32 {
    match input {
        "double" => |mut number| {
            number *= 2;
            println!("Doubling number. Now it is {}", number);
            number
        },
        "triple" => |mut number| {
            number *= 40;
            println!("Tripling number. Now it is {}", number);
            number
        },
        _ => |number| {
            println!("Sorry, it's the same: {}.", number);
            number
        },
    }
}

fn main() {
    let my_number = 10;

    // Make three closures
    let mut doubles = returns_a_closure("double");
    let mut triples = returns_a_closure("triple");
    let mut quadruples = returns_a_closure("quadruple");

    doubles(my_number);
    triples(my_number);
    quadruples(my_number);
}
```

下面是一个比较长的例子。让我们想象一下，在一个游戏中，你的角色面对的是晚上比较强的怪物。我们可以创建一个叫`TimeOfDay`的枚举来记录一天的情况。你的角色叫西蒙，有一个叫`character_fear`的数字，也就是`f64`。它晚上上升，白天下降。我们将创建一个`change_fear`函数，改变他的恐惧，但也做其他事情，如写消息。它大概是这样的:


```rust
enum TimeOfDay { // just a simple enum
    Dawn,
    Day,
    Sunset,
    Night,
}

fn change_fear(input: TimeOfDay) -> impl FnMut(f64) -> f64 { // The function takes a TimeOfDay. It returns a closure.
                                                             // We use impl FnMut(64) -> f64 to say that it needs to
                                                             // change the value, and also gives the same type back.
    use TimeOfDay::*; // So we only have to write Dawn, Day, Sunset, Night
                      // Instead of TimeOfDay::Dawn, TimeOfDay::Day, etc.
    match input {
        Dawn => |x| { // This is the variable character_fear that we give it later
            println!("The morning sun has vanquished the horrible night. You no longer feel afraid.");
            println!("Your fear is now {}", x * 0.5);
            x * 0.5
        },
        Day => |x| {
            println!("What a nice day. Maybe put your feet up and rest a bit.");
            println!("Your fear is now {}", x * 0.2);
            x * 0.2
        },
        Sunset => |x| {
            println!("The sun is almost down! This is no good.");
            println!("Your fear is now {}", x * 1.4);
            x * 1.4
        },
        Night => |x| {
            println!("What a horrible night to have a curse.");
            println!("Your fear is now {}", x * 5.0);
            x * 5.0
        },
    }
}

fn main() {
    use TimeOfDay::*;
    let mut character_fear = 10.0; // Start Simon with 10

    let mut daytime = change_fear(Day); // Make four closures here to call every time we want to change Simon's fear.
    let mut sunset = change_fear(Sunset);
    let mut night = change_fear(Night);
    let mut morning = change_fear(Dawn);

    character_fear = daytime(character_fear); // Call the closures on Simon's fear. They give a message and change the fear number.
                                              // In real life we would have a Character struct and use it as a method instead,
                                              // like this: character_fear.daytime()
    character_fear = sunset(character_fear);
    character_fear = night(character_fear);
    character_fear = morning(character_fear);
}
```

这个打印:

```text
What a nice day. Maybe put your feet up and rest a bit.
Your fear is now 2
The sun is almost down! This is no good.
Your fear is now 2.8
What a horrible night to have a curse.
Your fear is now 14
The morning sun has vanquished the horrible night. You no longer feel afraid.
Your fear is now 7
```

## Arc

你还记得我们用`Rc`来给一个变量一个以上的所有者。如果我们在线程中做同样的事情，我们需要一个 `Arc`。`Arc`的意思是 "atomic reference counter"(原子引用计数器)。原子的意思是它使用计算机的处理器，所以每次只写一次数据。这一点很重要，因为如果两个线程同时写入数据，你会得到错误的结果。例如，想象一下，如果你能在Rust中做到这一点。

```rust
// 🚧
let mut x = 10;

for i in 0..10 { // Thread 1
    x += 1
}
for i in 0..10 { // Thread 2
    x += 1
}
```


如果线程1和线程2一起启动，也许就会出现这种情况。

- 线程1看到10，写下11，然后线程2看到11，写下12 然后线程2看到11，写入12。到目前为止没有问题。
- 线程1看到12。同时，线程2看到12。线程一看到13，写下13 线程2也写了13 现在我们有13个，但应该是14个 Now we have 13, but it should be 14. 这是个大问题。

`Arc`使用处理器来确保这种情况不会发生，所以当你有线程时必须使用这种方法。不过不建议单线程上用`Arc`，因为`Rc`更快一些。

不过你不能只用一个`Arc`来改变数据。所以你用一个`Mutex`把数据包起来，然后用一个`Arc`把`Mutex`包起来。

所以我们用一个`Mutex`在一个`Arc`里面来改变一个数字的值。首先我们设置一个线程。

```rust
fn main() {

    let handle = std::thread::spawn(|| {
        println!("The thread is working!") // Just testing the thread
    });

    handle.join().unwrap(); // Make the thread wait here until it is done
    println!("Exiting the program");
}
```

到目前为止，这个只打印:

```text
The thread is working!
Exiting the program
```

很好，现在让我们把它放在`for`的循环中，进行`0..5`。

```rust
fn main() {

    let handle = std::thread::spawn(|| {
        for _ in 0..5 {
            println!("The thread is working!")
        }
    });

    handle.join().unwrap();
    println!("Exiting the program");
}
```

这也是可行的。我们得到以下结果:

```text
The thread is working!
The thread is working!
The thread is working!
The thread is working!
The thread is working!
Exiting the program
```

现在我们再加一个线程。每个线程都会做同样的事情。你可以看到，这些线程是在同一时间工作的。有时会先打印`Thread 1 is working!`，但其他时候`Thread 2 is working!`先打印。这就是所谓的**并发**，也就是 "一起运行"的意思。

```rust
fn main() {

    let thread1 = std::thread::spawn(|| {
        for _ in 0..5 {
            println!("Thread 1 is working!")
        }
    });

    let thread2 = std::thread::spawn(|| {
        for _ in 0..5 {
            println!("Thread 2 is working!")
        }
    });

    thread1.join().unwrap();
    thread2.join().unwrap();
    println!("Exiting the program");
}
```

这将打印:

```text
Thread 1 is working!
Thread 1 is working!
Thread 1 is working!
Thread 1 is working!
Thread 1 is working!
Thread 2 is working!
Thread 2 is working!
Thread 2 is working!
Thread 2 is working!
Thread 2 is working!
Exiting the program
```

现在我们要改变`my_number`的数值。现在它是一个`i32`。我们将把它改为 `Arc<Mutex<i32>>`:一个可以改变的 `i32`，由 `Arc` 保护。

```rust
// 🚧
let my_number = Arc::new(Mutex::new(0));
```

现在我们有了这个，我们可以克隆它。每个克隆可以进入不同的线程。我们有两个线程，所以我们将做两个克隆。

```rust
// 🚧
let my_number = Arc::new(Mutex::new(0));

let my_number1 = Arc::clone(&my_number); // This clone goes into Thread 1
let my_number2 = Arc::clone(&my_number); // This clone goes into Thread 2
```

现在，我们已经将安全克隆连接到`my_number`，我们可以将它们`move`到其他线程中，没有问题。

```rust
use std::sync::{Arc, Mutex};

fn main() {
    let my_number = Arc::new(Mutex::new(0));

    let my_number1 = Arc::clone(&my_number);
    let my_number2 = Arc::clone(&my_number);

    let thread1 = std::thread::spawn(move || { // Only the clone goes into Thread 1
        for _ in 0..10 {
            *my_number1.lock().unwrap() +=1; // Lock the Mutex, change the value
        }
    });

    let thread2 = std::thread::spawn(move || { // Only the clone goes into Thread 2
        for _ in 0..10 {
            *my_number2.lock().unwrap() += 1;
        }
    });

    thread1.join().unwrap();
    thread2.join().unwrap();
    println!("Value is: {:?}", my_number);
    println!("Exiting the program");
}
```

程序打印:

```text
Value is: Mutex { data: 20 }
Exiting the program
```

所以这是一个成功的案例。

然后我们可以将两个线程连接在一起，形成一个`for`循环，并使代码更短。

我们需要保存句柄，这样我们就可以在循环外对每个线程调用`.join()`。如果我们在循环内这样做，它将等待第一个线程完成后再启动新的线程。

```rust
use std::sync::{Arc, Mutex};

fn main() {
    let my_number = Arc::new(Mutex::new(0));
    let mut handle_vec = vec![]; // JoinHandles will go in here

    for _ in 0..2 { // do this twice
        let my_number_clone = Arc::clone(&my_number); // Make the clone before starting the thread
        let handle = std::thread::spawn(move || { // Put the clone in
            for _ in 0..10 {
                *my_number_clone.lock().unwrap() += 1;
            }
        });
        handle_vec.push(handle); // save the handle so we can call join on it outside of the loop
                                 // If we don't push it in the vec, it will just die here
    }

    handle_vec.into_iter().for_each(|handle| handle.join().unwrap()); // call join on all handles
    println!("{:?}", my_number);
}
```

最后这个打印`Mutex { data: 20 }`。

这看起来很复杂，但`Arc<Mutex<SomeType>>>`在Rust中使用的频率很高，所以它变得很自然。另外，你也可以随时写你的代码，让它更干净。这里是同样的代码，多了一条`use`语句和两个函数。这些函数并没有做任何新的事情，但是它们把一些代码从`main()`中移出。如果你很难读懂的话，可以尝试重写这样的代码。

```rust
use std::sync::{Arc, Mutex};
use std::thread::spawn; // Now we just write spawn

fn make_arc(number: i32) -> Arc<Mutex<i32>> { // Just a function to make a Mutex in an Arc
    Arc::new(Mutex::new(number))
}

fn new_clone(input: &Arc<Mutex<i32>>) -> Arc<Mutex<i32>> { // Just a function so we can write new_clone
    Arc::clone(&input)
}

// Now main() is easier to read
fn main() {
    let mut handle_vec = vec![]; // each handle will go in here
    let my_number = make_arc(0);

    for _ in 0..2 {
        let my_number_clone = new_clone(&my_number);
        let handle = spawn(move || {
            for _ in 0..10 {
                let mut value_inside = my_number_clone.lock().unwrap();
                *value_inside += 1;
            }
        });
        handle_vec.push(handle);    // the handle is done, so put it in the vector
    }

    handle_vec.into_iter().for_each(|handle| handle.join().unwrap()); // Make each one wait

    println!("{:?}", my_number);
}
```

## Channels

A channel is an easy way to use many threads that send to one place.它们相当流行，因为它们很容易组合在一起。你可以在Rust中用`std::sync::mpsc`创建一个channel。`mpsc`的意思是 "多个生产者，单个消费者"，所以 "many threads sending to one place"。要启动一个通道，你可以使用 `channel()`。这将创建一个 `Sender` 和一个 `Receiver`，它们被绑在一起。你可以在函数签名中看到这一点。

```rust
// 🚧
pub fn channel<T>() -> (Sender<T>, Receiver<T>)
```

所以你要选择一个发送者的名字和一个接收者的名字。通常你会看到像`let (sender, receiver) = channel();`这样的开头。因为它是泛型函数，如果你只写这个，Rust不会知道类型。

```rust
use std::sync::mpsc::channel;

fn main() {
    let (sender, receiver) = channel(); // ⚠️
}
```

编译器说:

```text
error[E0282]: type annotations needed for `(std::sync::mpsc::Sender<T>, std::sync::mpsc::Receiver<T>)`
  --> src\main.rs:30:30
   |
30 |     let (sender, receiver) = channel();
   |         ------------------   ^^^^^^^ cannot infer type for type parameter `T` declared on the function `channel`
   |         |
   |         consider giving this pattern the explicit type `(std::sync::mpsc::Sender<T>, std::sync::mpsc::Receiver<T>)`, where
the type parameter `T` is specified
```

它建议为`Sender`和`Receiver`添加一个类型。如果你愿意的话，可以这样做:

```rust
use std::sync::mpsc::{channel, Sender, Receiver}; // Added Sender and Receiver here

fn main() {
    let (sender, receiver): (Sender<i32>, Receiver<i32>) = channel();
}
```

但你不必这样做: 一旦你开始使用`Sender`和`Receiver`，Rust就能猜到类型。

所以我们来看一下最简单的使用通道的方法。

```rust
use std::sync::mpsc::channel;

fn main() {
    let (sender, receiver) = channel();

    sender.send(5);
    receiver.recv(); // recv = receive, not "rec v"
}
```

现在编译器知道类型了。`sender`是`Result<(), SendError<i32>>`，`receiver`是`Result<i32, RecvError>`。所以你可以用`.unwrap()`来看看发送是否有效，或者使用更好的错误处理。我们加上`.unwrap()`，也加上`println!`，看看得到什么。

```rust
use std::sync::mpsc::channel;

fn main() {
    let (sender, receiver) = channel();

    sender.send(5).unwrap();
    println!("{}", receiver.recv().unwrap());
}
```

这样就可以打印出`5`。

`channel`就像`Arc`一样，因为你可以克隆它，并将克隆的内容发送到其他线程中。让我们创建两个线程，并将值发送到`receiver`。这段代码可以工作，但它并不完全是我们想要的。

```rust
use std::sync::mpsc::channel;

fn main() {
    let (sender, receiver) = channel();
    let sender_clone = sender.clone();

    std::thread::spawn(move|| { // move sender in
        sender.send("Send a &str this time").unwrap();
    });

    std::thread::spawn(move|| { // move sender_clone in
        sender_clone.send("And here is another &str").unwrap();
    });

    println!("{}", receiver.recv().unwrap());
}
```

两个线程开始发送，然后我们`println!`。它可能会打印 `Send a &str this time` 或 `And here is another &str`，这取决于哪个线程先完成。让我们创建一个join句柄来等待它们完成。

```rust
use std::sync::mpsc::channel;

fn main() {
    let (sender, receiver) = channel();
    let sender_clone = sender.clone();
    let mut handle_vec = vec![]; // Put our handles in here

    handle_vec.push(std::thread::spawn(move|| {  // push this into the vec
        sender.send("Send a &str this time").unwrap();
    }));

    handle_vec.push(std::thread::spawn(move|| {  // and push this into the vec
        sender_clone.send("And here is another &str").unwrap();
    }));

    for _ in handle_vec { // now handle_vec has 2 items. Let's print them
        println!("{:?}", receiver.recv().unwrap());
    }
}
```

这个将打印:

```text
"Send a &str this time"
"And here is another &str"
```

现在我们不打印，我们创建一个`results_vec`。

```rust
use std::sync::mpsc::channel;

fn main() {
    let (sender, receiver) = channel();
    let sender_clone = sender.clone();
    let mut handle_vec = vec![];
    let mut results_vec = vec![];

    handle_vec.push(std::thread::spawn(move|| {
        sender.send("Send a &str this time").unwrap();
    }));

    handle_vec.push(std::thread::spawn(move|| {
        sender_clone.send("And here is another &str").unwrap();
    }));

    for _ in handle_vec {
        results_vec.push(receiver.recv().unwrap());
    }

    println!("{:?}", results_vec);
}
```

现在结果在我们的vec中:`["Send a &str this time", "And here is another &str"]`。

现在让我们假设我们有很多工作要做，并且想要使用线程。我们有一个大的VEC，里面有1百万个元素，都是0，我们想把每个0都变成1，我们将使用10个线程，每个线程将做十分之一的工作。我们将创建一个新的VEC，并使用`.extend()`来收集结果。

```rust
use std::sync::mpsc::channel;
use std::thread::spawn;

fn main() {
    let (sender, receiver) = channel();
    let hugevec = vec![0; 1_000_000];
    let mut newvec = vec![];
    let mut handle_vec = vec![];

    for i in 0..10 {
        let sender_clone = sender.clone();
        let mut work: Vec<u8> = Vec::with_capacity(hugevec.len() / 10); // new vec to put the work in. 1/10th the size
        work.extend(&hugevec[i*100_000..(i+1)*100_000]); // first part gets 0..100_000, next gets 100_000..200_000, etc.
        let handle =spawn(move || { // make a handle

            for number in work.iter_mut() { // do the actual work
                *number += 1;
            };
            sender_clone.send(work).unwrap(); // use the sender_clone to send the work to the receiver
        });
        handle_vec.push(handle);
    }

    for handle in handle_vec { // stop until the threads are done
        handle.join().unwrap();
    }

    while let Ok(results) = receiver.try_recv() {
        newvec.push(results); // push the results from receiver.recv() into the vec
    }

    // Now we have a Vec<Vec<u8>>. To put it together we can use .flatten()
    let newvec = newvec.into_iter().flatten().collect::<Vec<u8>>(); // Now it's one vec of 1_000_000 u8 numbers

    println!("{:?}, {:?}, total length: {}", // Let's print out some numbers to make sure they are all 1
        &newvec[0..10], &newvec[newvec.len()-10..newvec.len()], newvec.len() // And show that the length is 1_000_000 items
    );

    for number in newvec { // And let's tell Rust that it can panic if even one number is not 1
        if number != 1 {
            panic!();
        }
    }
}
```

## 阅读Rust文档

知道如何阅读Rust中的文档是很重要的，这样你就可以理解其他人写的东西。这里有一些Rust文档中需要知道的事情。

### assert_eq!


你在做测试的时候看到`assert_eq!`是用的。你把两个元素放在函数里面，如果它们不相等，程序就会崩溃。下面是一个简单的例子，我们需要一个偶数。

```rust
fn main() {
    prints_number(56);
}

fn prints_number(input: i32) {
    assert_eq!(input % 2, 0); // number must be equal.
                              // If number % 2 is not 0, it panics
    println!("The number is not odd. It is {}", input);
}
```

也许你没有任何计划在你的代码中使用`assert_eq!`，但它在Rust文档中随处可见。这是因为在一个文档中，你需要很大的空间来`println!`一切。另外，你会需要`Display`或`Debug`来打印你想打印的东西。这就是为什么文档中到处都有`assert_eq!`的原因。下面是这里的一个例子[https://doc.rust-lang.org/std/vec/struct.Vec.html](https://doc.rust-lang.org/std/vec/struct.Vec.html)，展示了如何使用Vec。

```rust
fn main() {
    let mut vec = Vec::new();
    vec.push(1);
    vec.push(2);

    assert_eq!(vec.len(), 2);
    assert_eq!(vec[0], 1);

    assert_eq!(vec.pop(), Some(2));
    assert_eq!(vec.len(), 1);

    vec[0] = 7;
    assert_eq!(vec[0], 7);

    vec.extend([1, 2, 3].iter().copied());

    for x in &vec {
        println!("{}", x);
    }
    assert_eq!(vec, [7, 1, 2, 3]);
}
```

在这些例子中，你可以只把`assert_eq!(a, b)`看成是在说 "a是b"。现在看看右边带有注释的同一个例子。注释显示了它的实际含义。

```rust
fn main() {
    let mut vec = Vec::new();
    vec.push(1);
    vec.push(2);

    assert_eq!(vec.len(), 2); // "The vec length is 2"
    assert_eq!(vec[0], 1); // "vec[0] is 1"

    assert_eq!(vec.pop(), Some(2)); // "When you use .pop(), you get Some()"
    assert_eq!(vec.len(), 1); // "The vec length is now 1"

    vec[0] = 7;
    assert_eq!(vec[0], 7); // "Vec[0] is 7"

    vec.extend([1, 2, 3].iter().copied());

    for x in &vec {
        println!("{}", x);
    }
    assert_eq!(vec, [7, 1, 2, 3]); // "The vec now has [7, 1, 2, 3]"
}
```

### 搜索

Rust 文档的顶部栏是搜索栏。它在你输入时显示结果。当你往下翻时，你不能再看到搜索栏，但如果你按键盘上的**s**键，你可以再次搜索。所以在任何地方按**s**键可以让你马上搜索。

### [src] 按钮

通常一个方法、结构体等的代码不会是完整的。这是因为你通常不需要看到完整的源码就能知道它是如何工作的，而完整的代码可能会让人困惑。但如果你想知道更多，你可以点击[src]就可以看到所有的内容。例如，在`String`的页面上，你可以看到`.with_capacity()`的这个签名。

```rust
// 🚧
pub fn with_capacity(capacity: usize) -> String
```

好了，你输入一个数字，它给你一个`String`。这很简单，但也许我们很好奇，想看更多。如果你点击[src]你可以看到这个。

```rust
// 🚧
pub fn with_capacity(capacity: usize) -> String {
    String { vec: Vec::with_capacity(capacity) }
}
```

有趣的是，现在你可以看到，字符串是`Vec`的一种。而实际上一个`String`是一个`u8`字节的向量，这很有意思。你不需要知道，就可以使用`with_capacity`的方法，你只有点击[src]才能看到。所以如果文档没有太多细节，而你又想知道更多的话，点击[src]是个好主意。

### trait信息

trait文档的重要部分是左边的 "Required Methods"。如果你看到 "Required Methods"，可能意味着你必须自己编写方法。例如，对于 `Iterator`，你需要写 `.next()` 方法。而对于`From`，你需要写`.from()`方法。但是有些trait只需要一个**属性**就可以实现，比如我们在`#[derive(Debug)]`中看到的。`Debug`需要`.fmt()`方法，但通常你只需要使用`#[derive(Debug)]`，除非你想自己做。这就是为什么在`std::fmt::Debug`的页面上说 "一般来说，你应该直接派生出一个Debug实现"。

## 属性

你以前见过`#[derive(Debug)]`这样的代码:这种类型的代码叫做*属性*。这些属性是给编译器提供信息的小段代码。它们不容易创建，但使用起来非常方便。如果你只用`#`写一个属性，那么它将影响下一行的代码。但如果你用`#!`来写，那么它将影响自己空间里的一切。

下面是一些你会经常看到的属性。

`#[allow(dead_code)]` 和 `#[allow(unused_variables)]`。 如果你写了不用的代码，Rust仍然会编译，但会让你知道。例如，这里有一个结构体，里面什么都没有，只有一个变量。我们不使用它们中的任何一个。

```rust
struct JustAStruct {}

fn main() {
    let some_char = 'ん';
}
```

如果你这样写，Rust会提醒你，你没有使用它们。

```text
warning: unused variable: `some_char`
 --> src\main.rs:4:9
  |
4 |     let some_char = 'ん';
  |         ^^^^^^^^^ help: if this is intentional, prefix it with an underscore: `_some_char`
  |
  = note: `#[warn(unused_variables)]` on by default

warning: struct is never constructed: `JustAStruct`
 --> src\main.rs:1:8
  |
1 | struct JustAStruct {}
  |        ^^^^^^^^^^^
  |
  = note: `#[warn(dead_code)]` on by default
```

我们知道，可以在名字前写一个`_`，让编译器安静下来。

```rust
struct _JustAStruct {}

fn main() {
    let _some_char = 'ん';
}
```

但你也可以使用属性。你会注意到在消息中，它使用了`#[warn(unused_variables)]`和`#[warn(dead_code)]`。在我们的代码中，`JustAStruct`是死代码，而`some_char`是一个未使用的变量。`warn`的反义词是`allow`，所以我们可以这样写，它不会说什么。

```rust
#![allow(dead_code)]
#![allow(unused_variables)]

struct Struct1 {} // Create five structs
struct Struct2 {}
struct Struct3 {}
struct Struct4 {}
struct Struct5 {}

fn main() {
    let char1 = 'ん'; // and four variables. We don't use any of them but the compiler is quiet
    let char2 = ';';
    let some_str = "I'm just a regular &str";
    let some_vec = vec!["I", "am", "just", "a", "vec"];
}
```

当然，处理死代码和未使用的变量是很重要的。但有时你希望编译器安静一段时间。或者您可能需要展示一些代码或教人们Rust，但又不想用编译器的信息来迷惑他们。

`#[derive(TraitName)]`让你可以为你创建的结构和枚举派生一些trait。这适用于许多可以自动派生的常见trait。有些像 `Display` 这样的特性不能自动衍生，因为对于 `Display`，你必须选择如何显示。

```rust
// ⚠️
#[derive(Display)]
struct HoldsAString {
    the_string: String,
}

fn main() {
    let my_string = HoldsAString {
        the_string: "Here I am!".to_string(),
    };
}
```

错误信息会告诉你:

```text
error: cannot find derive macro `Display` in this scope
 --> src\main.rs:2:10
  |
2 | #[derive(Display)]
  |
```

但是对于可以自动推导出的trait，你可以随心所欲的放进去。让我们给`HoldsAString`在一行中加入七个trait，只是为了好玩，尽管它只需要一个。

```rust
#[derive(Debug, PartialEq, Eq, Ord, PartialOrd, Hash, Clone)]
struct HoldsAString {
    the_string: String,
}

fn main() {
    let my_string = HoldsAString {
        the_string: "Here I am!".to_string(),
    };
    println!("{:?}", my_string);
}
```

另外，如果(也只有在)它的字段都实现了`Copy`的情况下，你才可以创建一个`Copy`结构。`HoldsAString`包含`String`，它没有实现`Copy`，所以你不能对它使用`#[derive(Copy)]`。但是对下面这个结构你可以:

```rust
#[derive(Clone, Copy)] // You also need Clone to use Copy
struct NumberAndBool {
    number: i32, // i32 is Copy
    true_or_false: bool // bool is also Copy. So no problem
}

fn does_nothing(input: NumberAndBool) {

}

fn main() {
    let number_and_bool = NumberAndBool {
        number: 8,
        true_or_false: true
    };

    does_nothing(number_and_bool);
    does_nothing(number_and_bool); // If it didn't have copy, this would make an error
}
```


`#[cfg()]`的意思是配置，告诉编译器是否运行代码。它通常是这样的:`#[cfg(test)]`。你在写测试函数的时候用这个，这样它就知道除非你在测试，否则不要运行它们。那么你可以在你的代码附近写测试，但编译器不会运行它们，除非你告诉编译器。

还有一个使用`cfg`的例子是`#[cfg(target_os = "windows")]`。有了它，你可以告诉编译器只在Windows，Linux或其他平台则不能运行代码。

`#![no_std]`是一个有趣的属性，它告诉Rust不要引入标准库。这意味着你没有`Vec`，`String`，以及标准库中的其他任何东西。你会在那些没有多少内存或空间的小型设备的代码中看到这个。

你可以在[这里](https://doc.rust-lang.org/reference/attributes.html)看到更多的属性。


## Box

`Box` 是 Rust 中一个非常方便的类型。当你使用`Box`时，你可以把一个类型放在堆上而不是栈上。要创建一个新的 `Box`，只需使用 `Box::new()` 并将元素放在里面即可。

```rust
fn just_takes_a_variable<T>(item: T) {} // Takes anything and drops it.

fn main() {
    let my_number = 1; // This is an i32
    just_takes_a_variable(my_number);
    just_takes_a_variable(my_number); // Using this function twice is no problem, because it's Copy

    let my_box = Box::new(1); // This is a Box<i32>
    just_takes_a_variable(my_box.clone()); // Without .clone() the second function would make an error
    just_takes_a_variable(my_box); // because Box is not Copy
}
```

一开始很难想象在哪里使用它，但你在Rust中经常使用它。你记得`&`是用于`str`的，因为编译器不知道`str`的大小:它可以是任何长度。但是`&`的引用总是相同的长度，所以编译器可以使用它。`Box`也是类似的。另外，你也可以在`Box`上使用`*`来获取值，就像使用`&`一样。

```rust
fn main() {
    let my_box = Box::new(1); // This is a Box<i32>
    let an_integer = *my_box; // This is an i32
    println!("{:?}", my_box);
    println!("{:?}", an_integer);
}
```

这就是为什么Box被称为 "智能指针"的原因，因为它就像`&`的引用(指针的一种)，但可以做更多的事情。

你也可以使用Box来创建里面有相同结构的结构体。这些结构被称为*递归*，这意味着在Struct A里面也许是另一个Struct A，有时你可以使用Box来创建链表，尽管这在Rust中并不十分流行。但如果你想创建一个递归结构，你可以使用`Box`。如果你试着不用 `Box` 会发生什么:


```rust
struct List {
    item: Option<List>, // ⚠️
}
```

这个简单的`List`有一项，可能是`Some<List>`(另一个列表)，也可能是`None`。因为你可以选择`None`，所以它不会永远递归。但是编译器还是不知道大小。

```text
error[E0072]: recursive type `List` has infinite size
  --> src\main.rs:16:1
   |
16 | struct List {
   | ^^^^^^^^^^^ recursive type has infinite size
17 |     item: Option<List>,
   |     ------------------ recursive without indirection
   |
   = help: insert indirection (e.g., a `Box`, `Rc`, or `&`) at some point to make `List` representable
```

你可以看到，它甚至建议尝试`Box`。所以我们用`Box`把List包裹起来。

```rust
struct List {
    item: Option<Box<List>>,
}
fn main() {}
```

现在编译器用`List`就可以了，因为所有的东西都在`Box`后面，而且它知道`Box`的大小。那么一个非常简单的列表可能是这样的:

```rust
struct List {
    item: Option<Box<List>>,
}

impl List {
    fn new() -> List {
        List {
            item: Some(Box::new(List { item: None })),
        }
    }
}

fn main() {
    let mut my_list = List::new();
}
```

即使没有数据也有点复杂，Rust并不怎么使用这种类型的模式。这是因为Rust对借用和所有权有严格的规定，你知道的。但如果你想启动一个这样的列表(链表)，`Box`可以帮助你。

`Box`还可以让你在上面使用`std::mem::drop`，因为它在堆上。这有时会很方便。

## 用Box包裹trait

`Box`对于返回trait非常有用。你可以像这个例子一样用泛型函数写trait:

```rust
use std::fmt::Display;

struct DoesntImplementDisplay {}

fn displays_it<T: Display>(input: T) {
    println!("{}", input);
}

fn main() {}
```

这个只能接受`Display`的东西，所以它不能接受我们的`DoesntImplementDisplay`结构。但是它可以接受很多其他的东西，比如`String`。

你也看到了，我们可以使用 `impl Trait` 来返回其他的trait，或者闭包。`Box`也可以用类似的方式使用。你可以使用 `Box`，否则编译器将不知道值的大小。这个例子表明，trait可以用在任何大小的东西上:

```rust
#![allow(dead_code)] // Tell the compiler to be quiet
use std::mem::size_of; // This gives the size of a type

trait JustATrait {} // We will implement this on everything

enum EnumOfNumbers {
    I8(i8),
    AnotherI8(i8),
    OneMoreI8(i8),
}
impl JustATrait for EnumOfNumbers {}

struct StructOfNumbers {
    an_i8: i8,
    another_i8: i8,
    one_more_i8: i8,
}
impl JustATrait for StructOfNumbers {}

enum EnumOfOtherTypes {
    I8(i8),
    AnotherI8(i8),
    Collection(Vec<String>),
}
impl JustATrait for EnumOfOtherTypes {}

struct StructOfOtherTypes {
    an_i8: i8,
    another_i8: i8,
    a_collection: Vec<String>,
}
impl JustATrait for StructOfOtherTypes {}

struct ArrayAndI8 {
    array: [i8; 1000], // This one will be very large
    an_i8: i8,
    in_u8: u8,
}
impl JustATrait for ArrayAndI8 {}

fn main() {
    println!(
        "{}, {}, {}, {}, {}",
        size_of::<EnumOfNumbers>(),
        size_of::<StructOfNumbers>(),
        size_of::<EnumOfOtherTypes>(),
        size_of::<StructOfOtherTypes>(),
        size_of::<ArrayAndI8>(),
    );
}
```

当我们打印这些东西的size的时候，我们得到`2, 3, 32, 32, 1002`。所以如果你像下面这样做的话，会得到一个错误：

```rust
// ⚠️
fn returns_just_a_trait() -> JustATrait {
    let some_enum = EnumOfNumbers::I8(8);
    some_enum
}
```

它说：

```text
error[E0746]: return type cannot have an unboxed trait object
  --> src\main.rs:53:30
   |
53 | fn returns_just_a_trait() -> JustATrait {
   |                              ^^^^^^^^^^ doesn't have a size known at compile-time
```

而这是真的，因为size可以是2，3，32，1002，或者其他任何东西。所以我们把它放在一个`Box`中。在这里我们还要加上`dyn`这个关键词。`dyn`这个词告诉你，你说的是一个trait，而不是一个结构体或其他任何东西。

所以你可以把函数改成这样。

```rust
// 🚧
fn returns_just_a_trait() -> Box<dyn JustATrait> {
    let some_enum = EnumOfNumbers::I8(8);
    Box::new(some_enum)
}
```

现在它工作了，因为在栈上只是一个`Box`，我们知道`Box`的大小。

你会经常看到`Box<dyn Error>`这种形式，因为有时你可能会有多个可能的错误。

我们可以快速创建两个错误类型来显示这一点。要创建一个正式的错误类型，你必须为它实现`std::error::Error`。这部分很容易:只要写出 `impl std::error::Error {}`。但错误还需要`Debug`和`Display`，这样才能给出问题的信息。`Debug`只要加上`#[derive(Debug)]`就行，很容易，但`Display`需要`.fmt()`方法。我们之前做过一次。

代码是这样的:

```rust
use std::error::Error;
use std::fmt;

#[derive(Debug)]
struct ErrorOne;

impl Error for ErrorOne {} // Now it is an error type with Debug. Time for Display:

impl fmt::Display for ErrorOne {
    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
        write!(f, "You got the first error!") // All it does is write this message
    }
}


#[derive(Debug)] // Do the same thing with ErrorTwo
struct ErrorTwo;

impl Error for ErrorTwo {}

impl fmt::Display for ErrorTwo {
    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
        write!(f, "You got the second error!")
    }
}

// Make a function that just returns a String or an error
fn returns_errors(input: u8) -> Result<String, Box<dyn Error>> { // With Box<dyn Error> you can return anything that has the Error trait

    match input {
        0 => Err(Box::new(ErrorOne)), // Don't forget to put it in a box
        1 => Err(Box::new(ErrorTwo)),
        _ => Ok("Looks fine to me".to_string()), // This is the success type
    }

}

fn main() {

    let vec_of_u8s = vec![0_u8, 1, 80]; // Three numbers to try out

    for number in vec_of_u8s {
        match returns_errors(number) {
            Ok(input) => println!("{}", input),
            Err(message) => println!("{}", message),
        }
    }
}
```

这将打印:

```text
You got the first error!
You got the second error!
Looks fine to me
```

如果我们没有`Box<dyn Error>`，写了这个，我们就有问题了。

```rust
// ⚠️
fn returns_errors(input: u8) -> Result<String, Error> {
    match input {
        0 => Err(ErrorOne),
        1 => Err(ErrorTwo),
        _ => Ok("Looks fine to me".to_string()),
    }
}
```

它会告诉你。

```text
21  | fn returns_errors(input: u8) -> Result<String, Error> {
    |                                 ^^^^^^^^^^^^^^^^^^^^^ doesn't have a size known at compile-time
```

这并不奇怪，因为我们知道，一个trait可以作用于很多东西，而且它们各自有不同的大小。

## 默认值和建造者模式


你可以实现 `Default` trait，给你认为最常见的 `struct` 或 `enum` 赋值。建造者模式可以很好地与之配合，让用户在需要时轻松地进行修改。首先我们来看看`Default`。实际上，Rust中的大多数通用类型已经有`Default`。它们并不奇怪。0, ""(空字符串), `false`, 等等。

```rust
fn main() {
    let default_i8: i8 = Default::default();
    let default_str: String = Default::default();
    let default_bool: bool = Default::default();

    println!("'{}', '{}', '{}'", default_i8, default_str, default_bool);
}
```

这将打印`'0', '', 'false'`。

所以`Default`就像`new`函数一样，除了你不需要输入任何东西。首先我们要创建一个`struct`，它还没有实现`Default`。它有一个`new`函数，我们用它来创建一个名为Billy的角色，并提供一些统计信息。

```rust
struct Character {
    name: String,
    age: u8,
    height: u32,
    weight: u32,
    lifestate: LifeState,
}

enum LifeState {
    Alive,
    Dead,
    NeverAlive,
    Uncertain
}

impl Character {
    fn new(name: String, age: u8, height: u32, weight: u32, alive: bool) -> Self {
        Self {
            name,
            age,
            height,
            weight,
            lifestate: if alive { LifeState::Alive } else { LifeState::Dead },
        }
    }
}

fn main() {
    let character_1 = Character::new("Billy".to_string(), 15, 170, 70, true);
}
```

但也许在我们的世界里，我们希望大部分角色都叫比利，年龄15岁，身高170，体重70，还活着。我们可以实现`Default`，这样我们就可以直接写`Character::default()`。它看起来是这样的:

```rust
#[derive(Debug)]
struct Character {
    name: String,
    age: u8,
    height: u32,
    weight: u32,
    lifestate: LifeState,
}

#[derive(Debug)]
enum LifeState {
    Alive,
    Dead,
    NeverAlive,
    Uncertain,
}

impl Character {
    fn new(name: String, age: u8, height: u32, weight: u32, alive: bool) -> Self {
        Self {
            name,
            age,
            height,
            weight,
            lifestate: if alive {
                LifeState::Alive
            } else {
                LifeState::Dead
            },
        }
    }
}

impl Default for Character {
    fn default() -> Self {
        Self {
            name: "Billy".to_string(),
            age: 15,
            height: 170,
            weight: 70,
            lifestate: LifeState::Alive,
        }
    }
}

fn main() {
    let character_1 = Character::default();

    println!(
        "The character {:?} is {:?} years old.",
        character_1.name, character_1.age
    );
}
```

打印出`The character "Billy" is 15 years old.`，简单多了!

现在我们来看建造者模式。我们会有很多Billy，所以我们会保留默认的。但是很多其他角色只会有一点不同。建造者模式让我们可以把小方法链接起来，每次改变一个值。这里是一个`Character`的方法:

```rust
fn height(mut self, height: u32) -> Self {    // 🚧
    self.height = height;
    self
}
```

一定要注意，它取的是`mut self`。我们之前看到过一次，它不是一个可变引用(`&mut self`)。它占用了`Self`的所有权，有了`mut`，它将是可变的，即使它之前不是可变的。这是因为`.height()`拥有完全的所有权，别人不能碰它，所以它是安全的，可变。它只是改变`self.height`，然后返回`Self`(就是`Character`)。

所以我们有三个这样的构建方法。它们几乎是一样的:

```rust
fn height(mut self, height: u32) -> Self {     // 🚧
    self.height = height;
    self
}

fn weight(mut self, weight: u32) -> Self {
    self.weight = weight;
    self
}

fn name(mut self, name: &str) -> Self {
    self.name = name.to_string();
    self
}
```

每一个都会改变一个变量，并回馈给`Self`:这就是你在建造者模式中看到的。所以现在我们类似这样写来创建一个角色:`let character_1 = Character::default().height(180).weight(60).name("Bobby");`。如果你正在构建一个库给别人使用，这可以让他们很容易用起来。对最终用户来说很容易，因为它几乎看起来像自然的英语。"给我一个默认角色，身高为180，体重为60，名字为Bobby." 到目前为止，我们的代码看起来是这样的:

```rust
#[derive(Debug)]
struct Character {
    name: String,
    age: u8,
    height: u32,
    weight: u32,
    lifestate: LifeState,
}

#[derive(Debug)]
enum LifeState {
    Alive,
    Dead,
    NeverAlive,
    Uncertain,
}

impl Character {
    fn new(name: String, age: u8, height: u32, weight: u32, alive: bool) -> Self {
        Self {
            name,
            age,
            height,
            weight,
            lifestate: if alive {
                LifeState::Alive
            } else {
                LifeState::Dead
            },
        }
    }

    fn height(mut self, height: u32) -> Self {
        self.height = height;
        self
    }

    fn weight(mut self, weight: u32) -> Self {
        self.weight = weight;
        self
    }

    fn name(mut self, name: &str) -> Self {
        self.name = name.to_string();
        self
    }
}

impl Default for Character {
    fn default() -> Self {
        Self {
            name: "Billy".to_string(),
            age: 15,
            height: 170,
            weight: 70,
            lifestate: LifeState::Alive,
        }
    }
}

fn main() {
    let character_1 = Character::default().height(180).weight(60).name("Bobby");

    println!("{:?}", character_1);
}
```

最后一个要添加的方法通常叫`.build()`。这个方法是一种最终检查。当你给用户提供一个像`.height()`这样的方法时，你可以确保他们只输入一个`u32()`，但是如果他们输入5000的身高怎么办？这在你正在做的游戏中可能就不对了。我们最后将使用一个名为`.build()`的方法，返回一个`Result`。在它里面我们将检查用户输入是否正常，如果正常，我们将返回一个 `Ok(Self)`。

不过首先我们要改变`.new()`方法。我们不希望用户再自由创建任何一种角色。所以我们将把`impl Default`的值移到`.new()`。而现在`.new()`不接受任何输入。

```rust
    fn new() -> Self {    // 🚧
        Self {
            name: "Billy".to_string(),
            age: 15,
            height: 170,
            weight: 70,
            lifestate: LifeState::Alive,
        }
    }
```

这意味着我们不再需要`impl Default`了，因为`.new()`有所有的默认值。所以我们可以删除`impl Default`。

现在我们的代码是这样的。

```rust
#[derive(Debug)]
struct Character {
    name: String,
    age: u8,
    height: u32,
    weight: u32,
    lifestate: LifeState,
}

#[derive(Debug)]
enum LifeState {
    Alive,
    Dead,
    NeverAlive,
    Uncertain,
}

impl Character {
    fn new() -> Self {
        Self {
            name: "Billy".to_string(),
            age: 15,
            height: 170,
            weight: 70,
            lifestate: LifeState::Alive,
        }
    }

    fn height(mut self, height: u32) -> Self {
        self.height = height;
        self
    }

    fn weight(mut self, weight: u32) -> Self {
        self.weight = weight;
        self
    }

    fn name(mut self, name: &str) -> Self {
        self.name = name.to_string();
        self
    }
}

fn main() {
    let character_1 = Character::new().height(180).weight(60).name("Bobby");

    println!("{:?}", character_1);
}
```

这样打印出来的结果是一样的:`Character { name: "Bobby", age: 15, height: 180, weight: 60, lifestate: Alive }`。

我们几乎已经准备好写`.build()`方法了，但是有一个问题:如何让用户使用它？现在用户可以写`let x = Character::new().height(76767);`，然后得到一个`Character`。有很多方法可以做到这一点，也许你能想出自己的方法。但是我们会在`Character`中增加一个`can_use: bool`的值。

```rust
#[derive(Debug)]       // 🚧
struct Character {
    name: String,
    age: u8,
    height: u32,
    weight: u32,
    lifestate: LifeState,
    can_use: bool, // Set whether the user can use the character
}

\\ Cut other code

    fn new() -> Self {
        Self {
            name: "Billy".to_string(),
            age: 15,
            height: 170,
            weight: 70,
            lifestate: LifeState::Alive,
            can_use: true, // .new() always gives a good character, so it's true
        }
    }
```

而对于其他的方法，比如`.height()`，我们会将`can_use`设置为`false`。只有`.build()`会再次设置为`true`，所以现在用户要用`.build()`做最后的检查。我们要确保`height`不高于200，`weight`不高于300。另外，在我们的游戏中，有一个不好的字叫`smurf`，我们不希望任何角色使用它。

我们的`.build()`方法是这样的:

```rust
fn build(mut self) -> Result<Character, String> {      // 🚧
    if self.height < 200 && self.weight < 300 && !self.name.to_lowercase().contains("smurf") {
        self.can_use = true;
        Ok(self)
    } else {
        Err("Could not create character. Characters must have:
1) Height below 200
2) Weight below 300
3) A name that is not Smurf (that is a bad word)"
            .to_string())
    }
}
```

`!self.name.to_lowercase().contains("smurf")` 确保用户不会写出类似 "SMURF"或 "IamSmurf"的字样。它让整个 `String` 都变成小写(小字母)，并检查 `.contains()` 而不是 `==`。而前面的`!`表示 "不是"。

如果一切正常，我们就把`can_use`设置为`true`，然后把`Ok`里面的字符给用户。

现在我们的代码已经完成了，我们将创建三个不工作的角色，和一个工作的角色。最后的代码是这样的。

```rust
#[derive(Debug)]
struct Character {
    name: String,
    age: u8,
    height: u32,
    weight: u32,
    lifestate: LifeState,
    can_use: bool, // Here is the new value
}

#[derive(Debug)]
enum LifeState {
    Alive,
    Dead,
    NeverAlive,
    Uncertain,
}

impl Character {
    fn new() -> Self {
        Self {
            name: "Billy".to_string(),
            age: 15,
            height: 170,
            weight: 70,
            lifestate: LifeState::Alive,
            can_use: true,  // .new() makes a fine character, so it is true
        }
    }

    fn height(mut self, height: u32) -> Self {
        self.height = height;
        self.can_use = false; // Now the user can't use the character
        self
    }

    fn weight(mut self, weight: u32) -> Self {
        self.weight = weight;
        self.can_use = false;
        self
    }

    fn name(mut self, name: &str) -> Self {
        self.name = name.to_string();
        self.can_use = false;
        self
    }

    fn build(mut self) -> Result<Character, String> {
        if self.height < 200 && self.weight < 300 && !self.name.to_lowercase().contains("smurf") {
            self.can_use = true;   // Everything is okay, so set to true
            Ok(self)               // and return the character
        } else {
            Err("Could not create character. Characters must have:
1) Height below 200
2) Weight below 300
3) A name that is not Smurf (that is a bad word)"
                .to_string())
        }
    }
}

fn main() {
    let character_with_smurf = Character::new().name("Lol I am Smurf!!").build(); // This one contains "smurf" - not okay
    let character_too_tall = Character::new().height(400).build(); // Too tall - not okay
    let character_too_heavy = Character::new().weight(500).build(); // Too heavy - not okay
    let okay_character = Character::new()
        .name("Billybrobby")
        .height(180)
        .weight(100)
        .build();   // This character is okay. Name is fine, height and weight are fine

    // Now they are not Character, they are Result<Character, String>. So let's put them in a Vec so we can see them:
    let character_vec = vec![character_with_smurf, character_too_tall, character_too_heavy, okay_character];

    for character in character_vec { // Now we will print the character if it's Ok, and print the error if it's Err
        match character {
            Ok(character_info) => println!("{:?}", character_info),
            Err(err_info) => println!("{}", err_info),
        }
        println!(); // Then add one more line
    }
}
```

这将打印:

```text
Could not create character. Characters must have:
1) Height below 200
2) Weight below 300
3) A name that is not Smurf (that is a bad word)

Could not create character. Characters must have:
1) Height below 200
2) Weight below 300
3) A name that is not Smurf (that is a bad word)

Could not create character. Characters must have:
1) Height below 200
2) Weight below 300
3) A name that is not Smurf (that is a bad word)

Character { name: "Billybrobby", age: 15, height: 180, weight: 100, lifestate: Alive, can_use: true }
```



## Deref和DerefMut

`Deref`是让你用`*`来解引用某些东西的trait。我们知道，一个引用和一个值是不一样的。

```rust
// ⚠️
fn main() {
    let value = 7; // This is an i32
    let reference = &7; // This is a &i32
    println!("{}", value == reference);
}
```

而Rust连`false`都不给，因为它甚至不会比较两者。

```text
error[E0277]: can't compare `{integer}` with `&{integer}`
 --> src\main.rs:4:26
  |
4 |     println!("{}", value == reference);
  |                          ^^ no implementation for `{integer} == &{integer}`
```

当然，这里的解法是使用`*`。所以这将打印出`true`。

```rust
fn main() {
    let value = 7;
    let reference = &7;
    println!("{}", value == *reference);
}
```


现在让我们想象一下一个简单的类型，它只是容纳一个数字。它就像一个`Box`，我们有一些想法为它提供一些额外的功能。但如果我们只是给它一个数字，
 它就不能做那么多了。

我们不能像使用`Box`那样使用`*`:

```rust
// ⚠️
struct HoldsANumber(u8);

fn main() {
    let my_number = HoldsANumber(20);
    println!("{}", *my_number + 20);
}
```

错误信息是:

```text
error[E0614]: type `HoldsANumber` cannot be dereferenced
  --> src\main.rs:24:22
   |
24 |     println!("{:?}", *my_number + 20);
```

我们当然可以做到这一点。`println!("{:?}", my_number.0 + 20);`. 但是这样的话，我们就是在20的基础上再单独加一个`u8`。如果我们能把它们加在一起就更好了。`cannot be dereferenced`这个消息给了我们一个线索:我们需要实现`Deref`。实现`Deref`的简单东西有时被称为 "智能指针"。一个智能指针可以指向它的元素，有它的信息，并且可以使用它的方法。因为现在我们可以添加`my_number.0`，这是一个`u8`，但我们不能用`HoldsANumber`做其他的事情:到目前为止，它只有`Debug`。

有趣的是:`String`其实是`&str`的智能指针，`Vec`是数组(或其他类型)的智能指针。所以我们其实从一开始就在使用智能指针。

实现`Deref`并不难，标准库中的例子也很简单。[下面是标准库中的示例代码](https://doc.rust-lang.org/std/ops/trait.Deref.html)。

```rust
use std::ops::Deref;

struct DerefExample<T> {
    value: T
}

impl<T> Deref for DerefExample<T> {
    type Target = T;

    fn deref(&self) -> &Self::Target {
        &self.value
    }
}

fn main() {
    let x = DerefExample { value: 'a' };
    assert_eq!('a', *x);
}
```


所以我们按照这个来，现在我们的`Deref`是这样的。

```rust
// 🚧
impl Deref for HoldsANumber {
    type Target = u8; // Remember, this is the "associated type": the type that goes together.
                      // You have to use the right type Target = (the type you want to return)

    fn deref(&self) -> &Self::Target { // Rust calls .deref() when you use *. We just defined Target as a u8 so this is easy to understand
        &self.0   // We chose &self.0 because it's a tuple struct. In a named struct it would be something like "&self.number"
    }
}
```

所以现在我们可以用`*`来做:

```rust
use std::ops::Deref;
#[derive(Debug)]
struct HoldsANumber(u8);

impl Deref for HoldsANumber {
    type Target = u8;

    fn deref(&self) -> &Self::Target {
        &self.0
    }
}

fn main() {
    let my_number = HoldsANumber(20);
    println!("{:?}", *my_number + 20);
}
```

所以，这样就可以打印出`40`，我们不需要写`my_number.0`。这意味着我们得到了 `u8` 的方法，我们可以为 `HoldsANumber` 写出我们自己的方法。我们将添加自己的简单方法，并使用我们从`u8`中得到的另一个方法，称为`.checked_sub()`。`.checked_sub()`方法是一个安全的减法，它能返回一个`Option`。如果它能做减法，那么它就会在`Some`里面给你，如果它不能做减法，那么它就会给出一个`None`。记住，`u8`不能是负数，所以还是`.checked_sub()`比较安全，这样就不会崩溃了。

```rust
use std::ops::Deref;

struct HoldsANumber(u8);

impl HoldsANumber {
    fn prints_the_number_times_two(&self) {
        println!("{}", self.0 * 2);
    }
}

impl Deref for HoldsANumber {
    type Target = u8;

    fn deref(&self) -> &Self::Target {
        &self.0
    }
}

fn main() {
    let my_number = HoldsANumber(20);
    println!("{:?}", my_number.checked_sub(100)); // This method comes from u8
    my_number.prints_the_number_times_two(); // This is our own method
}
```

这个打印:

```text
None
40
```

我们也可以实现`DerefMut`，这样我们就可以通过`*`来改变数值。它看起来几乎是一样的。在实现`DerefMut`之前，你需要先实现`Deref`。

```rust
use std::ops::{Deref, DerefMut};

struct HoldsANumber(u8);

impl HoldsANumber {
    fn prints_the_number_times_two(&self) {
        println!("{}", self.0 * 2);
    }
}

impl Deref for HoldsANumber {
    type Target = u8;

    fn deref(&self) -> &Self::Target {
        &self.0
    }
}

impl DerefMut for HoldsANumber { // You don't need type Target = u8; here because it already knows thanks to Deref
    fn deref_mut(&mut self) -> &mut Self::Target { // Everything else is the same except it says mut everywhere
        &mut self.0
    }
}

fn main() {
    let mut my_number = HoldsANumber(20);
    *my_number = 30; // DerefMut lets us do this
    println!("{:?}", my_number.checked_sub(100));
    my_number.prints_the_number_times_two();
}
```

所以你可以看到，`Deref`给你的类型提供了强大的力量。

这也是为什么标准库说:`Deref should only be implemented for smart pointers to avoid confusion`。这是因为对于一个复杂的类型，你可以用 `Deref` 做一些奇怪的事情。让我们想象一个非常混乱的例子来理解它们的含义。我们将从一个游戏的 `Character` 结构开始。一个新的`Character`需要一些数据，比如智力和力量。所以这里是我们的第一个角色。

```rust
struct Character {
    name: String,
    strength: u8,
    dexterity: u8,
    health: u8,
    intelligence: u8,
    wisdom: u8,
    charm: u8,
    hit_points: i8,
    alignment: Alignment,
}

impl Character {
    fn new(
        name: String,
        strength: u8,
        dexterity: u8,
        health: u8,
        intelligence: u8,
        wisdom: u8,
        charm: u8,
        hit_points: i8,
        alignment: Alignment,
    ) -> Self {
        Self {
            name,
            strength,
            dexterity,
            health,
            intelligence,
            wisdom,
            charm,
            hit_points,
            alignment,
        }
    }
}

enum Alignment {
    Good,
    Neutral,
    Evil,
}

fn main() {
    let billy = Character::new("Billy".to_string(), 9, 8, 7, 10, 19, 19, 5, Alignment::Good);
}
```

现在让我们想象一下，我们要把人物的hit points放在一个大的vec里。也许我们会把怪物数据也放进去，把它放在一起。由于 `hit_points` 是一个 `i8`，我们实现了 `Deref`，所以我们可以对它进行各种计算。但是看看现在我们的`main()`函数中，它看起来多么奇怪。


```rust
use std::ops::Deref;

// All the other code is the same until after the enum Alignment
struct Character {
    name: String,
    strength: u8,
    dexterity: u8,
    health: u8,
    intelligence: u8,
    wisdom: u8,
    charm: u8,
    hit_points: i8,
    alignment: Alignment,
}

impl Character {
    fn new(
        name: String,
        strength: u8,
        dexterity: u8,
        health: u8,
        intelligence: u8,
        wisdom: u8,
        charm: u8,
        hit_points: i8,
        alignment: Alignment,
    ) -> Self {
        Self {
            name,
            strength,
            dexterity,
            health,
            intelligence,
            wisdom,
            charm,
            hit_points,
            alignment,
        }
    }
}

enum Alignment {
    Good,
    Neutral,
    Evil,
}

impl Deref for Character { // impl Deref for Character. Now we can do any integer math we want!
    type Target = i8;

    fn deref(&self) -> &Self::Target {
        &self.hit_points
    }
}



fn main() {
    let billy = Character::new("Billy".to_string(), 9, 8, 7, 10, 19, 19, 5, Alignment::Good); // Create two characters, billy and brandy
    let brandy = Character::new("Brandy".to_string(), 9, 8, 7, 10, 19, 19, 5, Alignment::Good);

    let mut hit_points_vec = vec![]; // Put our hit points data in here
    hit_points_vec.push(*billy);     // Push *billy?
    hit_points_vec.push(*brandy);    // Push *brandy?

    println!("{:?}", hit_points_vec);
}
```

这只打印了`[5, 5]`。我们的代码现在让人读起来感觉非常奇怪。我们可以在`main()`上面看到`Deref`，然后弄清楚`*billy`的意思是`i8`，但是如果有很多代码呢？可能我们的代码有2000行，突然要弄清楚为什么要`.push()` `*billy`。`Character`当然不仅仅是`i8`的智能指针。

当然，写`hit_points_vec.push(*billy)`并不违法，但这让代码看起来非常奇怪。也许一个简单的`.get_hp()`方法会好得多，或者另一个存放角色的结构体。然后你可以迭代并推送每个角色的 `hit_points`。`Deref`提供了很多功能，但最好确保代码的逻辑性。



## Crate和模块

每次你在 Rust 中写代码时，你都是在 `crate` 中写的。`crate`是一个或多个文件，一起为你的代码服务。在你写的文件里面，你也可以创建一个`mod`。`mod`是存放函数、结构体等的空间，因为这些原因被使用:

- 构建你的代码:它可以帮助你思考代码的总体结构。当你的代码越来越大时，这一点可能很重要。
- 阅读你的代码:人们可以更容易理解你的代码。例如，`std::collections::HashMap`这个名字告诉你，它在`std`的模块`collections`里面。这给了你一个提示，也许`collections`里面还有更多的集合类型，你可以尝试一下。
- 私密性:所有的东西一开始都是私有的。这样可以让你不让用户直接使用函数。

要创建一个`mod`，只需要写`mod`，然后用`{}`开始一个代码块。我们将创建一个名为`print_things`的mod，它有一些打印相关的功能。

```rust
mod print_things {
    use std::fmt::Display;

    fn prints_one_thing<T: Display>(input: T) { // Print anything that implements Display
        println!("{}", input)
    }
}

fn main() {}
```

你可以看到，我们把`use std::fmt::Display;`写在`print_things`里面，因为它是一个独立的空间。如果你把`use std::fmt::Display;`写在`main()`里面，那没用。而且，我们现在也不能从`main()`里面调用。如果在`fn`前面没有`pub`这个关键字，它就会保持私密性。让我们试着在没有`pub`的情况下调用它。这里有一种写法。

```rust
// 🚧
fn main() {
    crate::print_things::prints_one_thing(6);
}
```


`crate`的意思是 "在这个项目里"，但对于我们简单的例子来说，它和 "在这个文件里面"是一样的。接着是`print_things`这个mod，最后是`prints_one_thing()`函数。你可以每次都写这个，也可以写`use`来导入。现在我们可以看到说它是私有的错误:

```rust
// ⚠️
mod print_things {
    use std::fmt::Display;

    fn prints_one_thing<T: Display>(input: T) {
        println!("{}", input)
    }
}

fn main() {
    use crate::print_things::prints_one_thing;

    prints_one_thing(6);
    prints_one_thing("Trying to print a string...".to_string());
}
```

这是错误的。

```text
error[E0603]: function `prints_one_thing` is private
  --> src\main.rs:10:30
   |
10 |     use crate::print_things::prints_one_thing;
   |                              ^^^^^^^^^^^^^^^^ private function
   |
note: the function `prints_one_thing` is defined here
  --> src\main.rs:4:5
   |
4  |     fn prints_one_thing<T: Display>(input: T) {
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
```
很容易理解，函数`print_one_thing`是私有的。它还用`src\main.rs:4:5`告诉我们在哪里可以找到这个函数。这很有帮助，因为你不仅可以在一个文件中写`mod`，还可以在很多文件中写`mod`。

现在我们只需要写`pub fn`而不是`fn`，一切就都可以了。

```rust
mod print_things {
    use std::fmt::Display;

    pub fn prints_one_thing<T: Display>(input: T) {
        println!("{}", input)
    }
}

fn main() {
    use crate::print_things::prints_one_thing;

    prints_one_thing(6);
    prints_one_thing("Trying to print a string...".to_string());
}
```

这个打印:

```text
6
Trying to print a string...
```

`pub`对结构体、枚举、trait或模块有什么作用？`pub`对它们来说是这样的:

- `pub`对于一个结构：它使结构公开，但成员不是公开的。要想让一个成员公开，你也要为每个成员写`pub`。
- `pub` 对于一个枚举或trait：所有的东西都变成了公共的。这是有意义的，因为traits是给事物赋予相同的行为。而枚举是值之间的选择，你需要看到所有的枚举值才能做选择。
- `pub`对于一个模块来说：一个顶层的模块会是`pub`，因为如果它不是pub，那么根本没有人可以使用里面的任何东西。但是模块里面的模块需要使用`pub`才能成为公共的。

我们在`print_things`里面放一个名为`Billy`的结构体。这个结构体几乎都会是public的，但也不尽然。这个结构是公共的，所以它这样写：`pub struct Billy`。里面会有一个 `name` 和 `times_to_print`。`name`不会是公共的，因为我们只想让用户创建名为`"Billy".to_string()`的结构。但是用户可以选择打印的次数，所以这将是公开的。它的是这样的:

```rust
mod print_things {
    use std::fmt::{Display, Debug};

    #[derive(Debug)]
    pub struct Billy { // Billy is public
        name: String, // but name is private.
        pub times_to_print: u32,
    }

    impl Billy {
        pub fn new(times_to_print: u32) -> Self { // That means the user needs to use new to create a Billy. The user can only change the number of times_to_print
            Self {
                name: "Billy".to_string(), // We choose the name - the user can't
                times_to_print,
            }
        }

        pub fn print_billy(&self) { // This function prints a Billy
            for _ in 0..self.times_to_print {
                println!("{:?}", self.name);
            }
        }
    }

    pub fn prints_one_thing<T: Display>(input: T) {
        println!("{}", input)
    }
}

fn main() {
    use crate::print_things::*; // Now we use *. This imports everything from print_things

    let my_billy = Billy::new(3);
    my_billy.print_billy();
}
```

这将打印:

```text
"Billy"
"Billy"
"Billy"
```

对了，导入一切的`*`叫做 "glob运算符"。Glob的意思是 "全局"，所以它意味着一切。

在`mod`里面你可以创建其他mod。一个子 mod(mod里的mod)总是可以使用父 mod 内部的任何东西。你可以在下一个例子中看到这一点，我们在 `mod province` 里面有一个 `mod city`，而`mod province`在 `mod country` 里面。

你可以这样想:即使你在一个国家，你可能不在一个省。而即使你在一个省，你也可能不在一个市。但如果你在一个城市，你就在这个城市的省份和它的国家。


```rust
mod country { // The main mod doesn't need pub
    fn print_country(country: &str) { // Note: this function isn't public
        println!("We are in the country of {}", country);
    }
    pub mod province { // Make this mod public

        fn print_province(province: &str) { // Note: this function isn't public
            println!("in the province of {}", province);
        }

        pub mod city { // Make this mod public
            pub fn print_city(country: &str, province: &str, city: &str) {  // This function is public though
                crate::country::print_country(country);
                crate::country::province::print_province(province);
                println!("in the city of {}", city);
            }
        }
    }
}

fn main() {
    crate::country::province::city::print_city("Canada", "New Brunswick", "Moncton");
}
```

有趣的是，`print_city`可以访问`print_province`和`print_country`。这是因为`mod city`在其他mod里面。它不需要在`print_province`前面添加`pub`之后才能使用。这也是有道理的:一个城市不需要做什么，它本来就在一个省里，在一个国家里。

你可能注意到，`crate::country::province::print_province(province);`非常长。当我们在一个模块里面的时候，我们可以用`super`从上面引入元素。其实super这个词本身就是"上面"的意思，比如 "上级"。在我们的例子中，我们只用了一次函数，但是如果你用的比较多的话，那么最好是导入。如果它能让你的代码更容易阅读，那也是个好主意，即使你只用了一次函数。现在的代码几乎是一样的，但更容易阅读一些。

```rust
mod country {
    fn print_country(country: &str) {
        println!("We are in the country of {}", country);
    }
    pub mod province {
        fn print_province(province: &str) {
            println!("in the province of {}", province);
        }

        pub mod city {
            use super::super::*; // use everything in "above above": that means mod country
            use super::*;        // use everything in "above": that means mod province

            pub fn print_city(country: &str, province: &str, city: &str) {
                print_country(country);
                print_province(province);
                println!("in the city of {}", city);
            }
        }
    }
}

fn main() {
    use crate::country::province::city::print_city; // bring in the function

    print_city("Canada", "New Brunswick", "Moncton");
    print_city("Korea", "Gyeonggi-do", "Gwangju"); // Now it's less work to use it again
}
```



## 测试

现在我们已经了解了模块,就可以谈谈测试了。在Rust中测试你的代码是非常容易的，因为你可以在你的代码旁边写测试。

开始测试的最简单的方法是在一个函数上面添加`#[test]`。下面是一个简单的例子。

```rust
#[test]
fn two_is_two() {
    assert_eq!(2, 2);
}
```

但如果你试图在playground中运行它，它给出了一个错误。``error[E0601]: `main` function not found in crate `playground``. 这是因为你不使用 _Run_ 来进行测试，你使用 _Test_ 。另外，你不使用 `main()` 函数进行测试 - 它们在外面运行。要在Playground中运行这个，点击 _RUN_ 旁边的`···`，然后把它改为 _Test_ 。现在如果你点击它，它将运行测试。(如果你已经安装了 Rust，你将输入 `cargo test` 来做这个测试)

这里是输出:

```text
running 1 test
test two_is_two ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out
```

让我们把`assert_eq!(2, 2)`改成`assert_eq!(2, 3)`，看看会有什么结果。当测试失败时，你会得到更多的信息。

```text
running 1 test
test two_is_two ... FAILED

failures:

---- two_is_two stdout ----
thread 'two_is_two' panicked at 'assertion failed: `(left == right)`
  left: `2`,
 right: `3`', src/lib.rs:3:5
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace


failures:
    two_is_two

test result: FAILED. 0 passed; 1 failed; 0 ignored; 0 measured; 0 filtered out
```

`assert_eq!(left, right)`是Rust中测试一个函数的主要方法。如果它不工作，它将显示不同的值:左边有2，但右边有3。

`RUST_BACKTRACE=1`是什么意思？这是计算机上的一个设置，可以提供更多关于错误的信息。幸好playground也有:点击`STABLE`旁边的`···`，然后设置回溯为`ENABLED`。如果你这样做，它会给你*很多*的信息。

```text
running 1 test
test two_is_two ... FAILED

failures:

---- two_is_two stdout ----
thread 'two_is_two' panicked at 'assertion failed: 2 == 3', src/lib.rs:3:5
stack backtrace:
   0: backtrace::backtrace::libunwind::trace
             at /cargo/registry/src/github.com-1ecc6299db9ec823/backtrace-0.3.46/src/backtrace/libunwind.rs:86
   1: backtrace::backtrace::trace_unsynchronized
             at /cargo/registry/src/github.com-1ecc6299db9ec823/backtrace-0.3.46/src/backtrace/mod.rs:66
   2: std::sys_common::backtrace::_print_fmt
             at src/libstd/sys_common/backtrace.rs:78
   3: <std::sys_common::backtrace::_print::DisplayBacktrace as core::fmt::Display>::fmt
             at src/libstd/sys_common/backtrace.rs:59
   4: core::fmt::write
             at src/libcore/fmt/mod.rs:1076
   5: std::io::Write::write_fmt
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/libstd/io/mod.rs:1537
   6: std::io::impls::<impl std::io::Write for alloc::boxed::Box<W>>::write_fmt
             at src/libstd/io/impls.rs:176
   7: std::sys_common::backtrace::_print
             at src/libstd/sys_common/backtrace.rs:62
   8: std::sys_common::backtrace::print
             at src/libstd/sys_common/backtrace.rs:49
   9: std::panicking::default_hook::{{closure}}
             at src/libstd/panicking.rs:198
  10: std::panicking::default_hook
             at src/libstd/panicking.rs:215
  11: std::panicking::rust_panic_with_hook
             at src/libstd/panicking.rs:486
  12: std::panicking::begin_panic
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/libstd/panicking.rs:410
  13: playground::two_is_two
             at src/lib.rs:3
  14: playground::two_is_two::{{closure}}
             at src/lib.rs:2
  15: core::ops::function::FnOnce::call_once
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/libcore/ops/function.rs:232
  16: <alloc::boxed::Box<F> as core::ops::function::FnOnce<A>>::call_once
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/liballoc/boxed.rs:1076
  17: <std::panic::AssertUnwindSafe<F> as core::ops::function::FnOnce<()>>::call_once
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/libstd/panic.rs:318
  18: std::panicking::try::do_call
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/libstd/panicking.rs:297
  19: std::panicking::try
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/libstd/panicking.rs:274
  20: std::panic::catch_unwind
             at /rustc/c367798cfd3817ca6ae908ce675d1d99242af148/src/libstd/panic.rs:394
  21: test::run_test_in_process
             at src/libtest/lib.rs:541
  22: test::run_test::run_test_inner::{{closure}}
             at src/libtest/lib.rs:450
note: Some details are omitted, run with `RUST_BACKTRACE=full` for a verbose backtrace.


failures:
    two_is_two

test result: FAILED. 0 passed; 1 failed; 0 ignored; 0 measured; 0 filtered out
```

除非你真的找不到问题所在，否则你不需要使用回溯。但幸运的是你也不需要全部理解。 如果你继续阅读，你最终会看到第13行，那里写着`playground`--那是它提到的你的代码的位置。其他的都是关于Rust为了运行你的程序,在其他库中所做的事情。但是这两行告诉你，它看的是playground的第2行和第3行，这是一个提示，要检查那里。这里是那个部分:

```text
  13: playground::two_is_two
             at src/lib.rs:3
  14: playground::two_is_two::{{closure}}
             at src/lib.rs:2
```

编辑：Rust在2021年初改进了其回溯信息，只显示最有意义的信息。现在它更容易阅读。

```text
failures:

---- two_is_two stdout ----
thread 'two_is_two' panicked at 'assertion failed: `(left == right)`
  left: `2`,
 right: `3`', src/lib.rs:3:5
stack backtrace:
   0: rust_begin_unwind
             at /rustc/cb75ad5db02783e8b0222fee363c5f63f7e2cf5b/library/std/src/panicking.rs:493:5
   1: core::panicking::panic_fmt
             at /rustc/cb75ad5db02783e8b0222fee363c5f63f7e2cf5b/library/core/src/panicking.rs:92:14
   2: playground::two_is_two
             at ./src/lib.rs:3:5
   3: playground::two_is_two::{{closure}}
             at ./src/lib.rs:2:1
   4: core::ops::function::FnOnce::call_once
             at /rustc/cb75ad5db02783e8b0222fee363c5f63f7e2cf5b/library/core/src/ops/function.rs:227:5
   5: core::ops::function::FnOnce::call_once
             at /rustc/cb75ad5db02783e8b0222fee363c5f63f7e2cf5b/library/core/src/ops/function.rs:227:5
note: Some details are omitted, run with `RUST_BACKTRACE=full` for a verbose backtrace.


failures:
    two_is_two

test result: FAILED. 0 passed; 1 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.02s
```

现在我们再把回溯关闭，回到常规测试。现在我们要写一些其他函数，并使用测试函数来测试它们。这里有几个:

```rust
fn return_two() -> i8 {
    2
}
# [test]
fn it_returns_two() {
    assert_eq!(return_two(), 2);
}

fn return_six() -> i8 {
    4 + return_two()
}
# [test]
fn it_returns_six() {
    assert_eq!(return_six(), 6)
}
```

现在，都能运行:

```text
running 2 tests
test it_returns_two ... ok
test it_returns_six ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out
```

这不是太难。

通常你会想把你的测试放在自己的模块中。要做到这一点，请使用相同的 `mod` 关键字，并在其上方添加 `#[cfg(test)]`(记住:`cfg` 的意思是 "配置")。你还要在每个测试上面继续写`#[test]`。这是因为以后当你安装Rust时，你可以做更复杂的测试。你将可以运行一个测试，或者所有的测试，或者运行几个测试。另外别忘了写`use super::*;`，因为测试模块需要使用上面的函数。现在它看起来会是这样的。

```rust
fn return_two() -> i8 {
    2
}
fn return_six() -> i8 {
    4 + return_two()
}

# [cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn it_returns_six() {
        assert_eq!(return_six(), 6)
    }
    #[test]
    fn it_returns_two() {
        assert_eq!(return_two(), 2);
    }
}
```

### 测试驱动的开发

在阅读Rust或其他语言时，你可能会看到 "测试驱动开发"这个词。这是编写程序的一种方式，有些人喜欢它，而有些人则喜欢其他的方式。"测试驱动开发"的意思是 "先写测试，再写代码"。当你这样做的时候，你会有很多关于你想要你的代码做的所有事情的测试代码。然后你开始写代码，并运行测试，看看你是否做对了。然后，当你添加和重写代码时，如果有什么地方出了问题，测试代码会一直在那里向你展示。这在Rust中是非常容易的，因为编译器给出了很多待修复内容的信息。让我们写一个测试驱动开发的小例子，看看它是什么样子的。

让我们想象一个接受用户输入的计算器。它可以加(+)，也可以减(-)。如果用户写 "5+6"，它应该返回11，如果用户写 "5+6-7"，它应该返回4，以此类推。所以我们先从测试函数开始。你也可以看到，测试中的函数名通常都相当长。这是因为你可能会运行很多测试，你想了解哪些测试失败了。

我们想象一下，一个名为`math()`的函数就可以完成所有的工作。它将返回一个 `i32`(我们不会使用浮点数)。因为它需要返回一些东西，所以我们每次都只返回 `6`。然后我们将写三个测试函数。当然，它们都会失败。现在的代码是这样的。

```rust
fn math(input: &str) -> i32 {
    6
}

# [cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn one_plus_one_is_two() {
        assert_eq!(math("1 + 1"), 2);
    }
    #[test]
    fn one_minus_two_is_minus_one() {
        assert_eq!(math("1 - 2"), -1);
    }
    #[test]
    fn one_minus_minus_one_is_two() {
        assert_eq!(math("1 - -1"), 2);
    }
}
```

它给了我们这个信息。

```text
running 3 tests
test tests::one_minus_minus_one_is_two ... FAILED
test tests::one_minus_two_is_minus_one ... FAILED
test tests::one_plus_one_is_two ... FAILED
```

以及``thread 'tests::one_plus_one_is_two' panicked at 'assertion failed: `(left == right)` ``的所有信息。我们不需要在这里全部打印出来。

现在要考虑如何创建计算器。我们将接受任何数字，以及符号`+-`。我们将允许空格，但不允许其他任何东西。所以，让我们从包含所有数值的`const`开始。然后我们将使用 `.chars()` 按字符进行迭代，并使用 `.all()` 确保它们都在里面。

然后，我们将添加一个会崩溃的测试。要做到这一点，添加 `#[should_panic]` 属性:现在如果它崩溃，测试将成功。

现在代码看起来像这样:

```rust
const OKAY_CHARACTERS: &str = "1234567890+- "; // Don't forget the space at the end

fn math(input: &str) -> i32 {
    if !input.chars().all(|character| OKAY_CHARACTERS.contains(character)) {
        panic!("Please only input numbers, +-, or spaces");
    }
    6 // we still return a 6 for now
}

# [cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn one_plus_one_is_two() {
        assert_eq!(math("1 + 1"), 2);
    }
    #[test]
    fn one_minus_two_is_minus_one() {
        assert_eq!(math("1 - 2"), -1);
    }
    #[test]
    fn one_minus_minus_one_is_two() {
        assert_eq!(math("1 - -1"), 2);
    }

    #[test]
    #[should_panic]  // Here is our new test - it should panic
    fn panics_when_characters_not_right() {
        math("7 + seven");
    }
}
```

现在，当我们运行测试时，我们得到这样的结果。

```text
running 4 tests
test tests::one_minus_two_is_minus_one ... FAILED
test tests::one_minus_minus_one_is_two ... FAILED
test tests::panics_when_characters_not_right ... ok
test tests::one_plus_one_is_two ... FAILED
```

一个成功了! 我们的`math()`函数现在只能接受好的输入了。


下一步是编写实际的计算器。这就是先有测试的有趣之处:实际的代码要晚很多。首先，我们将把计算器的逻辑放在一起。我们要做到以下几点。

- 所有的空位都应该被删除。这在`.filter()`中很容易实现。
- 所有输入应该变成一个`Vec`。`+`不需要成为输入，但是当程序看到`+`时，应该知道这个数字已经完成了。例如，输入`+`应该这样做:
    1) 看到`1`，把它推到一个空字符串中。
    2) 看到另一个1，把它推入字符串中(现在是 "11")。
    3) 看到一个`+`，知道这个数字已经结束。它会把字符串推入vec中，然后清空字符串。
- 程序必须计算出`-`的数量。奇数(1，3，5...)表示减法，偶数(2，4，6...)表示加法。所以 "1--9"应该是10，而不是-8。
- 程序应该删除最后一个数字后面的任何东西。`5+5+++++----`是由`OKAY_CHARACTERS`中的所有字符组成的，但它应该变成`5+5`。`.trim_end_matches()`就很简单了，你把`&str`末尾符合的东西都去掉。

顺便说一下，`.trim_end_matches()`和`.trim_start_matches()`曾经是`trim_right_matches()`和`trim_left_matches()`。但后来人们注意到有些语言是从右到左(波斯语、希伯来语等)，所以左右都是错的。你可能还能在一些代码中看到旧的名字，但它们是一样的)。)

首先我们只想通过所有的测试。通过测试后，我们就可以 "重构"了。重构的意思是让代码变得更好，通常是通过结构、枚举和方法等方式。下面是我们使测试通过的代码。

```rust
const OKAY_CHARACTERS: &str = "1234567890+- ";

fn math(input: &str) -> i32 {
    if !input.chars().all(|character| OKAY_CHARACTERS.contains(character)) ||
       !input.chars().take(2).any(|character| character.is_numeric())
    {
        panic!("Please only input numbers, +-, or spaces.");
    }

    let input = input.trim_end_matches(|x| "+- ".contains(x)).chars().filter(|x| *x != ' ').collect::<String>(); // Remove + and - at the end, and all spaces
    let mut result_vec = vec![]; // Results go in here
    let mut push_string = String::new(); // This is the string we push in every time. We will keep reusing it in the loop.
    for character in input.chars() {
        match character {
            '+' => {
                if !push_string.is_empty() { // If the string is empty, we don't want to push "" into result_vec
                    result_vec.push(push_string.clone()); // But if it's not empty, it will be a number. Push it into the vec
                    push_string.clear(); // Then clear the string
                }
            },
            '-' => { // If we get a -,
                if push_string.contains('-') || push_string.is_empty() { // check to see if it's empty or has a -
                    push_string.push(character) // if so, then push it in
                } else { // otherwise, it will contain a number
                result_vec.push(push_string.clone()); // so push the number into result_vec, clear it and then push -
                push_string.clear();
                push_string.push(character);
                }
            },
            number => { // number here means "anything else that matches". We selected the name here
                if push_string.contains('-') { // We might have some - characters to push in first
                    result_vec.push(push_string.clone());
                    push_string.clear();
                    push_string.push(number);
                } else { // But if we don't, that means we can push the number in
                    push_string.push(number);
                }
            },
        }
    }
    result_vec.push(push_string); // Push one last time after the loop is over. Don't need to .clone() because we don't use it anymore

    let mut total = 0; // Now it's time to do math. Start with a total
    let mut adds = true; // true = add, false = subtract
    let mut math_iter = result_vec.into_iter();
    while let Some(entry) = math_iter.next() { // Iter through the items
        if entry.contains('-') { // If it has a - character, check if it's even or odd
            if entry.chars().count() % 2 == 1 {
                adds = match adds {
                    true => false,
                    false => true
                };
                continue; // Go to the next item
            } else {
                continue;
            }
        }
        if adds == true {
            total += entry.parse::<i32>().unwrap(); // If there is no '-', it must be a number. So we are safe to unwrap
        } else {
            total -= entry.parse::<i32>().unwrap();
            adds = true;  // After subtracting, reset adds to true.
        }
    }
    total // Finally, return the total
}
   /// We'll add a few more tests just to make sure

#[cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn one_plus_one_is_two() {
        assert_eq!(math("1 + 1"), 2);
    }
    #[test]
    fn one_minus_two_is_minus_one() {
        assert_eq!(math("1 - 2"), -1);
    }
    #[test]
    fn one_minus_minus_one_is_two() {
        assert_eq!(math("1 - -1"), 2);
    }
    #[test]
    fn nine_plus_nine_minus_nine_minus_nine_is_zero() {
        assert_eq!(math("9+9-9-9"), 0); // This is a new test
    }
    #[test]
    fn eight_minus_nine_plus_nine_is_eight_even_with_characters_on_the_end() {
        assert_eq!(math("8  - 9     +9-----+++++"), 8); // This is a new test
    }
    #[test]
    #[should_panic]
    fn panics_when_characters_not_right() {
        math("7 + seven");
    }
}
```

现在测试通过了!

```text
running 6 tests
test tests::one_minus_minus_one_is_two ... ok
test tests::nine_plus_nine_minus_nine_minus_nine_is_zero ... ok
test tests::one_minus_two_is_minus_one ... ok
test tests::eight_minus_nine_plus_nine_is_eight_even_with_characters_on_the_end ... ok
test tests::one_plus_one_is_two ... ok
test tests::panics_when_characters_not_right ... ok

test result: ok. 6 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out
```

你可以看到，在测试驱动的开发中，有一个来回的过程。它是这样的。

- 首先你要写出所有你能想到的测试
- 然后你开始写代码。
- 当你写代码的时候，你会有其他测试的想法。
- 你添加测试，你的测试随着你的发展而增长。你的测试越多，你的代码被检查的次数就越多。

当然，测试并不能检查所有的东西，认为 "通过所有测试=代码是完美的"是错误的。但是，测试对于你修改代码的时候是非常好的。如果你以后修改了代码，然后运行测试，如果其中一个测试不成功，你就会知道该怎么修复。

现在我们可以重写(重构)一下代码。一个好的方法是用clippy开始。如果你安装了Rust，那么你可以输入`cargo clippy`，如果你使用的是Playground，那么点击`TOOLS`，选择Clippy。Clippy会查看你的代码，并给你提示，让你的代码更简单。我们的代码没有任何错误，但它可以更好。

Clippy会告诉我们两件事。

```text
warning: this loop could be written as a `for` loop
  --> src/lib.rs:44:5
   |
44 |     while let Some(entry) = math_iter.next() { // Iter through the items
   |     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ help: try: `for entry in math_iter`
   |
   = note: `#[warn(clippy::while_let_on_iterator)]` on by default
   = help: for further information visit https://rust-lang.github.io/rust-clippy/master/index.html#while_let_on_iterator

warning: equality checks against true are unnecessary
  --> src/lib.rs:53:12
   |
53 |         if adds == true {
   |            ^^^^^^^^^^^^ help: try simplifying it as shown: `adds`
   |
   = note: `#[warn(clippy::bool_comparison)]` on by default
   = help: for further information visit https://rust-lang.github.io/rust-clippy/master/index.html#bool_comparison
```

这是真的:`for entry in math_iter`比`while let Some(entry) = math_iter.next()`简单得多。而`for`循环实际上是一个迭代器，所以我们没有任何理由写`.iter()`。谢谢你，clippy! 而且我们也不需要做`math_iter`:我们可以直接写`for entry in result_vec`。

现在我们将开始一些真正的重构。我们将创建一个 `Calculator` 结构体，而不是单独的变量。这将拥有我们使用的所有变量。我们将改变两个名字以使其更加清晰。`result_vec`将变成`results`，`push_string`将变成`current_input`(current的意思是 "现在")。而到目前为止，它只有一种方法:new。

```rust
// 🚧
#[derive(Clone)]
struct Calculator {
    results: Vec<String>,
    current_input: String,
    total: i32,
    adds: bool,
}

impl Calculator {
    fn new() -> Self {
        Self {
            results: vec![],
            current_input: String::new(),
            total: 0,
            adds: true,
        }
    }
}
```

现在我们的代码其实比较长，但更容易读懂。比如，`if adds`现在是`if calculator.adds`，这就跟读英文完全一样。它的样子是这样的:

```rust
#[derive(Clone)]
struct Calculator {
    results: Vec<String>,
    current_input: String,
    total: i32,
    adds: bool,
}

impl Calculator {
    fn new() -> Self {
        Self {
            results: vec![],
            current_input: String::new(),
            total: 0,
            adds: true,
        }
    }
}

const OKAY_CHARACTERS: &str = "1234567890+- ";

fn math(input: &str) -> i32 {
    if !input.chars().all(|character| OKAY_CHARACTERS.contains(character)) ||
       !input.chars().take(2).any(|character| character.is_numeric()) {
        panic!("Please only input numbers, +-, or spaces");
    }

    let input = input.trim_end_matches(|x| "+- ".contains(x)).chars().filter(|x| *x != ' ').collect::<String>();
    let mut calculator = Calculator::new();

    for character in input.chars() {
        match character {
            '+' => {
                if !calculator.current_input.is_empty() {
                    calculator.results.push(calculator.current_input.clone());
                    calculator.current_input.clear();
                }
            },
            '-' => {
                if calculator.current_input.contains('-') || calculator.current_input.is_empty() {
                    calculator.current_input.push(character)
                } else {
                calculator.results.push(calculator.current_input.clone());
                calculator.current_input.clear();
                calculator.current_input.push(character);
                }
            },
            number => {
                if calculator.current_input.contains('-') {
                    calculator.results.push(calculator.current_input.clone());
                    calculator.current_input.clear();
                    calculator.current_input.push(number);
                } else {
                    calculator.current_input.push(number);
                }
            },
        }
    }
    calculator.results.push(calculator.current_input);

    for entry in calculator.results {
        if entry.contains('-') {
            if entry.chars().count() % 2 == 1 {
                calculator.adds = match calculator.adds {
                    true => false,
                    false => true
                };
                continue;
            } else {
                continue;
            }
        }
        if calculator.adds {
            calculator.total += entry.parse::<i32>().unwrap();
        } else {
            calculator.total -= entry.parse::<i32>().unwrap();
            calculator.adds = true;
        }
    }
    calculator.total
}

#[cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn one_plus_one_is_two() {
        assert_eq!(math("1 + 1"), 2);
    }
    #[test]
    fn one_minus_two_is_minus_one() {
        assert_eq!(math("1 - 2"), -1);
    }
    #[test]
    fn one_minus_minus_one_is_two() {
        assert_eq!(math("1 - -1"), 2);
    }
    #[test]
    fn nine_plus_nine_minus_nine_minus_nine_is_zero() {
        assert_eq!(math("9+9-9-9"), 0);
    }
    #[test]
    fn eight_minus_nine_plus_nine_is_eight_even_with_characters_on_the_end() {
        assert_eq!(math("8  - 9     +9-----+++++"), 8);
    }
    #[test]
    #[should_panic]
    fn panics_when_characters_not_right() {
        math("7 + seven");
    }
}
```

最后我们增加两个新方法。一个叫做 `.clear()`，清除 `current_input()`。另一个叫做 `push_char()`，把输入推到 `current_input()` 上。这是我们重构后的代码。

```rust
#[derive(Clone)]
struct Calculator {
    results: Vec<String>,
    current_input: String,
    total: i32,
    adds: bool,
}

impl Calculator {
    fn new() -> Self {
        Self {
            results: vec![],
            current_input: String::new(),
            total: 0,
            adds: true,
        }
    }

    fn clear(&mut self) {
        self.current_input.clear();
    }

    fn push_char(&mut self, character: char) {
        self.current_input.push(character);
    }
}

const OKAY_CHARACTERS: &str = "1234567890+- ";

fn math(input: &str) -> i32 {
    if !input.chars().all(|character| OKAY_CHARACTERS.contains(character)) ||
       !input.chars().take(2).any(|character| character.is_numeric()) {
        panic!("Please only input numbers, +-, or spaces");
    }

    let input = input.trim_end_matches(|x| "+- ".contains(x)).chars().filter(|x| *x != ' ').collect::<String>();
    let mut calculator = Calculator::new();

    for character in input.chars() {
        match character {
            '+' => {
                if !calculator.current_input.is_empty() {
                    calculator.results.push(calculator.current_input.clone());
                    calculator.clear();
                }
            },
            '-' => {
                if calculator.current_input.contains('-') || calculator.current_input.is_empty() {
                    calculator.push_char(character)
                } else {
                calculator.results.push(calculator.current_input.clone());
                calculator.clear();
                calculator.push_char(character);
                }
            },
            number => {
                if calculator.current_input.contains('-') {
                    calculator.results.push(calculator.current_input.clone());
                    calculator.clear();
                    calculator.push_char(number);
                } else {
                    calculator.push_char(number);
                }
            },
        }
    }
    calculator.results.push(calculator.current_input);

    for entry in calculator.results {
        if entry.contains('-') {
            if entry.chars().count() % 2 == 1 {
                calculator.adds = match calculator.adds {
                    true => false,
                    false => true
                };
                continue;
            } else {
                continue;
            }
        }
        if calculator.adds {
            calculator.total += entry.parse::<i32>().unwrap();
        } else {
            calculator.total -= entry.parse::<i32>().unwrap();
            calculator.adds = true;
        }
    }
    calculator.total
}

#[cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn one_plus_one_is_two() {
        assert_eq!(math("1 + 1"), 2);
    }
    #[test]
    fn one_minus_two_is_minus_one() {
        assert_eq!(math("1 - 2"), -1);
    }
    #[test]
    fn one_minus_minus_one_is_two() {
        assert_eq!(math("1 - -1"), 2);
    }
    #[test]
    fn nine_plus_nine_minus_nine_minus_nine_is_zero() {
        assert_eq!(math("9+9-9-9"), 0);
    }
    #[test]
    fn eight_minus_nine_plus_nine_is_eight_even_with_characters_on_the_end() {
        assert_eq!(math("8  - 9     +9-----+++++"), 8);
    }
    #[test]
    #[should_panic]
    fn panics_when_characters_not_right() {
        math("7 + seven");
    }
}
```

现在大概已经够好了。我们可以写更多的方法，但是像`calculator.results.push(calculator.current_input.clone());`这样的行已经很清楚了。重构最好是在你完成后还能轻松阅读代码的时候。你不希望只是为了让代码变短而重构:例如，`clc.clr()`就比`calculator.clear()`差很多。



## 外部crate

外部crate的意思是 "别人的crate"。

在本节中，你*差不多*需要安装Rust，但我们仍然可以只使用Playground。现在我们要学习如何导入别人写的crate。这在Rust中很重要，原因有二。

- 导入其他的crate很容易，并且...
- Rust标准库是相当小的。

这意味着，在Rust中，很多基本功能都需要用到外部Crate，这很正常。我们的想法是，如果使用外部Crate很方便，那么你可以选择最好的一个。也许一个人会为一个功能创建一个crate，然后其他人会创建一个更好的crate。

在本书中，我们只看最流行的crate，也就是每个使用Rust的人都知道的crate。

要开始学习外部Crate，我们将从最常见的Crate开始。`rand`.

### rand

你有没有注意到，我们还没有使用任何随机数？那是因为随机数不在标准库中。但是有很多crate "几乎是标准库"，因为大家都在使用它们。在任何情况下，带入一个 crate 是非常容易的。如果你的电脑上有Rust，有一个叫`Cargo.toml`的文件，里面有这些信息。`Cargo.toml`文件在你启动时是这样的。

```text
[package]
name = "rust_book"
version = "0.1.0"
authors = ["David MacLeod"]
edition = "2018"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]
```

现在，如果你想添加`rand` crate，在`crates.io`上搜索它，这是所有crate的去处。这将带你到`https://crates.io/crates/rand`。当你点击那个，你可以看到一个屏幕，上面写着`Cargo.toml   rand = "0.7.3"`。你所要做的就是在[dependencies]下添加这样的内容:

```text
[package]
name = "rust_book"
version = "0.1.0"
authors = ["David MacLeod"]
edition = "2018"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]
rand = "0.7.3"
```

然后Cargo会帮你完成剩下的工作。然后你就可以在`rand`文档网站上开始编写像[本例代码](https://docs.rs/rand/0.7.3/rand/)这样的代码。要想进入文档，你可以点击[crates.io上的页面](https://crates.io/crates/rand)中的`docs`按钮。

关于Cargo的介绍就到这里了:我们现在使用的还只是playground。幸运的是，playground已经安装了前100个crate。所以你还不需要写进`Cargo.toml`。在playground上，你可以想象，它有一个这样的长长的列表，有100个crate。


```text
[dependencies]
rand = "0.7.3"
some_other_crate = "0.1.0"
another_nice_crate = "1.7"
```


也就是说，如果要使用`rand`，你可以直接这样做:

```rust
use rand; // This means the whole crate rand
          // On your computer you can't just write this;
          // you need to write in the Cargo.toml file first

fn main() {
    for _ in 0..5 {
        let random_u16 = rand::random::<u16>();
        print!("{} ", random_u16);
    }
}
```

每次都会打印不同的`u16`号码，比如`42266 52873 56528 46927 6867`。



`rand`中的主要功能是`random`和`thread_rng`(rng的意思是 "随机数发生器")。而实际上如果你看`random`，它说:"这只是`thread_rng().gen()`的一个快捷方式"。所以其实是`thread_rng`基本做完了一切。

下面是一个简单的例子，从1到10的数字。为了得到这些数字，我们在1到11之间使用`.gen_range()`。

```rust
use rand::{thread_rng, Rng}; // Or just use rand::*; if we are lazy

fn main() {
    let mut number_maker = thread_rng();
    for _ in 0..5 {
        print!("{} ", number_maker.gen_range(1, 11));
    }
}
```

这将打印出`7 2 4 8 6`这样的东西。

用随机数我们可以做一些有趣的事情，比如为游戏创建角色。我们将使用`rand`和其他一些我们知道的东西来创建它们。在这个游戏中，我们的角色有六种状态，用一个d6来表示他们。d6是一个立方体，当你投掷它时，它能给出1、2、3、4、5或6。每个角色都会掷三次d6，所以每个统计都在3到18之间。

但是有时候如果你的角色有一些低的东西，比如3或4，那就不公平了。比如说你的力量是3，你就不能拿东西。所以还有一种方法是用d6四次。你掷四次，然后扔掉最低的数字。所以如果你掷3，3，1，6，那么你保留3，3，6=12。我们也会把这个方法做出来，所以游戏的主人可以决定。

这是我们简单的角色创建器。我们为数据统计创建了一个`Character`结构，甚至还实现了`Display`来按照我们想要的方式打印。

```rust
use rand::{thread_rng, Rng}; // Or just use rand::*; if we are lazy
use std::fmt; // Going to impl Display for our character


struct Character {
    strength: u8,
    dexterity: u8,    // This means "body quickness"
    constitution: u8, // This means "health"
    intelligence: u8,
    wisdom: u8,
    charisma: u8, // This means "popularity with people"
}

fn three_die_six() -> u8 { // A "die" is the thing you throw to get the number
    let mut generator = thread_rng(); // Create our random number generator
    let mut stat = 0; // This is the total
    for _ in 0..3 {
        stat += generator.gen_range(1..=6); // Add each time
    }
    stat // Return the total
}

fn four_die_six() -> u8 {
    let mut generator = thread_rng();
    let mut results = vec![]; // First put the numbers in a vec
    for _ in 0..4 {
        results.push(generator.gen_range(1..=6));
    }
    results.sort(); // Now a result like [4, 3, 2, 6] becomes [2, 3, 4, 6]
    results.remove(0); // Now it would be [3, 4, 6]
    results.iter().sum() // Return this result
}

enum Dice {
    Three,
    Four
}

impl Character {
    fn new(dice: Dice) -> Self { // true for three dice, false for four
        match dice {
            Dice::Three => Self {
                strength: three_die_six(),
                dexterity: three_die_six(),
                constitution: three_die_six(),
                intelligence: three_die_six(),
                wisdom: three_die_six(),
                charisma: three_die_six(),
            },
            Dice::Four => Self {
                strength: four_die_six(),
                dexterity: four_die_six(),
                constitution: four_die_six(),
                intelligence: four_die_six(),
                wisdom: four_die_six(),
                charisma: four_die_six(),
            },
        }
    }
    fn display(&self) { // We can do this because we implemented Display below
        println!("{}", self);
        println!();
    }
}

impl fmt::Display for Character { // Just follow the code for in https://doc.rust-lang.org/std/fmt/trait.Display.html and change it a bit
    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
        write!(
            f,
            "Your character has these stats:
strength: {}
dexterity: {}
constitution: {}
intelligence: {}
wisdom: {}
charisma: {}",
            self.strength,
            self.dexterity,
            self.constitution,
            self.intelligence,
            self.wisdom,
            self.charisma
        )
    }
}



fn main() {
    let weak_billy = Character::new(Dice::Three);
    let strong_billy = Character::new(Dice::Four);
    weak_billy.display();
    strong_billy.display();
}
```

它会打印出这样的东西。

```rust
Your character has these stats:
strength: 9
dexterity: 15
constitution: 15
intelligence: 8
wisdom: 11
charisma: 9

Your character has these stats:
strength: 9
dexterity: 13
constitution: 14
intelligence: 16
wisdom: 16
charisma: 10
```

有四个骰子的角色通常在大多数事情上都会好一点。


### rayon

`rayon` 是一个流行的crate，它可以让你加快 Rust 代码的速度。它之所以受欢迎，是因为它无需像 `thread::spawn` 这样的东西就能创建线程。换句话说，它之所以受欢迎是因为它既有效又容易编写。比如说

- `.iter()`, `.iter_mut()`, `into_iter()`在rayon中是这样写的:
- `.par_iter()`, `.par_iter_mut()`, `par_into_iter()`. 所以你只要加上`par_`，你的代码就会变得快很多。(par的意思是 "并行")

其他方法也一样:`.chars()`就是`.par_chars()`，以此类推。

这里举个例子，一段简单的代码，却让计算机做了很多工作。
```rust
fn main() {
    let mut my_vec = vec![0; 200_000];
    my_vec.iter_mut().enumerate().for_each(|(index, number)| *number+=index+1);
    println!("{:?}", &my_vec[5000..5005]);
}
```

它创建了一个有20万项的向量:每一项都是0，然后调用`.enumerate()`来获取每个数字的索引，并将0改为索引号。它的打印时间太长，所以我们只打印5000到5004项。这在Rust中还是非常快的，但如果你愿意，你可以用Rayon让它更快。代码几乎是一样的。

```rust
use rayon::prelude::*; // Import rayon

fn main() {
    let mut my_vec = vec![0; 200_000];
    my_vec.par_iter_mut().enumerate().for_each(|(index, number)| *number+=index+1); // add par_ to iter_mut
    println!("{:?}", &my_vec[5000..5005]);
}
```

就这样了。`rayon`还有很多其他的方法来定制你想做的事情，但最简单的就是 "添加`_par`，让你的程序更快"。

### serde

`serde`是一个流行的crate，它可以在JSON、YAML等格式间相互转换。最常见的使用方法是通过创建一个`struct`，上面有两个属性。[它看起来是这样的](https://serde.rs/)。

```rust
#[derive(Serialize, Deserialize, Debug)]
struct Point {
    x: i32,
    y: i32,
}
```

`Serialize`和`Deserialize`trait是使转换变得简单的原因。(这也是`serde`这个名字的由来)如果你的结构体上有这两个trait，那么你只需要调用一个方法就可以把它转化为JSON或其他任何东西。

### regex

[regex](https://crates.io/crates/regex) crate 可以让你使用 [正则表达式](https://en.wikipedia.org/wiki/Regular_expression) 搜索文本。有了它，你可以通过一次搜索得到诸如 `colour`, `color`, `colours` 和 `colors` 的匹配信息。正则表达式是另一门语言，如果你想使用它们，也必须学会。

### chrono

[chrono](https://crates.io/crates/chrono)是为那些需要更多时间功能的人准备的主要crate。我们现在来看一下标准库，它有时间的功能，但是如果你需要更多的功能，那么这个crate是一个不错的选择。


## 标准库之旅

现在你已经知道了很多Rust的知识，你将能够理解标准库里面的大部分东西。它里面的代码已经不是那么可怕了。让我们来看看它里面一些我们还没有学过的部分。本篇游记将介绍标准库的大部分部分，你不需要安装Rust。我们将重温很多我们已经知道的内容，这样我们就可以更深入地学习它们。

### 数组

关于数组需要注意的一点是，它们没有实现`Iterator.`。这意味着，如果你有一个数组，你不能使用`for`。但是你可以对它们使用 `.iter()` 这样的方法。或者你可以使用`&`来得到一个切片。实际上，如果你尝试使用`for`，编译器会准确地告诉你。

```rust
fn main() {
    // ⚠️
    let my_cities = ["Beirut", "Tel Aviv", "Nicosia"];

    for city in my_cities {
        println!("{}", city);
    }
}
```

消息是:

```text
error[E0277]: `[&str; 3]` is not an iterator
 --> src\main.rs:5:17
  |
  |                 ^^^^^^^^^ borrow the array with `&` or call `.iter()` on it to iterate over it
```

所以让我们试试这两种方法。它们的结果是一样的。

```rust
fn main() {
    let my_cities = ["Beirut", "Tel Aviv", "Nicosia"];

    for city in &my_cities {
        println!("{}", city);
    }
    for city in my_cities.iter() {
        println!("{}", city);
    }
}
```

这个打印:

```text
Beirut
Tel Aviv
Nicosia
Beirut
Tel Aviv
Nicosia
```



如果你想从一个数组中获取变量，你可以把它们的名字放在 `[]` 中来解构它。这与在 `match` 语句中使用元组或从结构体中获取变量是一样的。

```rust
fn main() {
    let my_cities = ["Beirut", "Tel Aviv", "Nicosia"];
    let [city1, city2, city3] = my_cities;
    println!("{}", city1);
}
```

打印出`Beirut`.

### char

您可以使用`.escape_unicode()`的方法来获取`char`的Unicode号码。

```rust
fn main() {
    let korean_word = "청춘예찬";
    for character in korean_word.chars() {
        print!("{} ", character.escape_unicode());
    }
}
```


这将打印出 `u{ccad} u{cd98} u{c608} u{cc2c}`。


你可以使用 `From` trait从 `u8` 中得到一个字符，但对于 `u32`，你使用 `TryFrom`，因为它可能无法工作。`u32`中的数字比Unicode中的字符多很多。我们可以通过一个简单的演示来了解。

```rust
use std::convert::TryFrom; // You need to bring TryFrom in to use it
use rand::prelude::*;      // We will use random numbers too

fn main() {
    let some_character = char::from(99); // This one is easy - no need for TryFrom
    println!("{}", some_character);

    let mut random_generator = rand::thread_rng();
    // This will try 40,000 times to make a char from a u32.
    // The range is 0 (std::u32::MIN) to u32's highest number (std::u32::MAX). If it doesn't work, we will give it '-'.
    for _ in 0..40_000 {
        let bigger_character = char::try_from(random_generator.gen_range(std::u32::MIN..std::u32::MAX)).unwrap_or('-');
        print!("{}", bigger_character)
    }
}
```

几乎每次都会生成一个`-`。这是你会看到的那种输出的一部分。

```text
------------------------------------------------------------------------𤒰---------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
-------------------------------------------------------------춗--------------------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------
------------򇍜----------------------------------------------------
```

所以，你要用`TryFrom`是件好事。

另外，从2020年8月底开始，你现在可以从`char`中得到一个`String`。(`String`实现了`From<char>`)只要写`String::from()`，然后在里面放一个`char`。


### 整数

这些类型的数学方法有很多，另外还有一些其他的方法。下面是一些最有用的。



`.checked_add()`, `.checked_sub()`, `.checked_mul()`, `.checked_div()`. 如果你认为你可能会得到一个不适合类型的数字，这些都是不错的方法。它们会返回一个 `Option`，这样你就可以安全地检查你的数学计算是否正常，而不会让程序崩溃。

```rust
fn main() {
    let some_number = 200_u8;
    let other_number = 200_u8;

    println!("{:?}", some_number.checked_add(other_number));
    println!("{:?}", some_number.checked_add(1));
}
```

这个打印:

```text
None
Some(201)
```


你会注意到，在整数的页面上，经常说`rhs`。这意味着 "右边"，也就是你做一些数学运算时的右操作数。比如在`5 + 6`中，`5`在左边，`6`在右边，所以`6`就是`rhs`。这个不是关键词，但是你会经常看到，所以知道就好。

说到这里，我们来学习一下如何实现`Add`。在你实现了`Add`之后，你可以在你创建的类型上使用`+`。你需要自己实现`Add`，因为add可以表达很多意思。这是标准库页面中的例子。

```rust
use std::ops::Add; // first bring in Add

#[derive(Debug, Copy, Clone, PartialEq)] // PartialEq is probably the most important part here. You want to be able to compare numbers
struct Point {
    x: i32,
    y: i32,
}

impl Add for Point {
    type Output = Self; // Remember, this is called an "associated type": a "type that goes together".
                        // In this case it's just another Point

    fn add(self, other: Self) -> Self {
        Self {
            x: self.x + other.x,
            y: self.y + other.y,
        }
    }
}
```

现在让我们为自己的类型实现`Add`。让我们想象一下，我们想把两个国家加在一起，这样我们就可以比较它们的经济。它看起来像这样:

```rust
use std::fmt;
use std::ops::Add;

#[derive(Clone)]
struct Country {
    name: String,
    population: u32,
    gdp: u32, // This is the size of the economy
}

impl Country {
    fn new(name: &str, population: u32, gdp: u32) -> Self {
        Self {
            name: name.to_string(),
            population,
            gdp,
        }
    }
}

impl Add for Country {
    type Output = Self;

    fn add(self, other: Self) -> Self {
        Self {
            name: format!("{} and {}", self.name, other.name), // We will add the names together,
            population: self.population + other.population, // and the population,
            gdp: self.gdp + other.gdp,   // and the GDP
        }
    }
}

impl fmt::Display for Country {
    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
        write!(
            f,
            "In {} are {} people and a GDP of ${}", // Then we can print them all with just {}
            self.name, self.population, self.gdp
        )
    }
}

fn main() {
    let nauru = Country::new("Nauru", 10_670, 160_000_000);
    let vanuatu = Country::new("Vanuatu", 307_815, 820_000_000);
    let micronesia = Country::new("Micronesia", 104_468, 367_000_000);

    // We could have given Country a &str instead of a String for the name. But we would have to write lifetimes everywhere
    // and that would be too much for a small example. Better to just clone them when we call println!.
    println!("{}", nauru.clone());
    println!("{}", nauru.clone() + vanuatu.clone());
    println!("{}", nauru + vanuatu + micronesia);
}
```

这个打印:

```text
In Nauru are 10670 people and a GDP of $160000000
In Nauru and Vanuatu are 318485 people and a GDP of $980000000
In Nauru and Vanuatu and Micronesia are 422953 people and a GDP of $1347000000
```

以后在这段代码中，我们可以把`.fmt()`改成更容易阅读的数字显示。

另外三个叫`Sub`、`Mul`和`Div`，实现起来基本一样。`+=`、`-=`、`*=`和`/=`，只要加上`Assign`:`AddAssign`、`SubAssign`、`MulAssign`和`DivAssign`即可。你可以看到完整的列表[这里](https://doc.rust-lang.org/std/ops/index.html#structs)，因为还有很多。例如 `%` 被称为 `Rem`, `-` 被称为 `Neg`, 等等。


### 浮点数

`f32`和`f64`有非常多的方法，你在做数学计算的时候会用到。我们不看这些，但这里有一些你可能会用到的方法。它们分别是 `.floor()`, `.ceil()`, `.round()`, 和 `.trunc()`. 所有这些方法都返回一个 `f32` 或 `f64`，它像一个整数，小数点后面是 `0`。它们是这样做的。

- `.floor()`: 给你下一个最低的整数.
- `.ceil()`: 给你下一个最高的整数。
- `.round()`: 如果小数部分大于等于0.5，返回数值加1;如果小数部分小于0.5，返回相同数值。这就是所谓的四舍五入，因为它给你一个 "舍入"的数字(一个数字的简短形式)。
- `.trunc()`:只是把小数点号后的部分截掉。Truncate是 "截断"的意思。

这里有一个简单的函数来打印它们。

```rust
fn four_operations(input: f64) {
    println!(
"For the number {}:
floor: {}
ceiling: {}
rounded: {}
truncated: {}\n",
        input,
        input.floor(),
        input.ceil(),
        input.round(),
        input.trunc()
    );
}

fn main() {
    four_operations(9.1);
    four_operations(100.7);
    four_operations(-1.1);
    four_operations(-19.9);
}
```

这个打印:

```text
For the number 9.1:
floor: 9
ceiling: 10
rounded: 9 // because less than 9.5
truncated: 9

For the number 100.7:
floor: 100
ceiling: 101
rounded: 101 // because more than 100.5
truncated: 100

For the number -1.1:
floor: -2
ceiling: -1
rounded: -1
truncated: -1

For the number -19.9:
floor: -20
ceiling: -19
rounded: -20
truncated: -19
```

`f32` 和 `f64` 有一个叫做 `.max()` 和 `.min()` 的方法，可以得到两个数字中较大或较小的数字。(对于其他类型，你可以直接使用`std::cmp::max`和`std::cmp::min`。)下面是用`.fold()`来得到最高或最低数的方法。你又可以看到，`.fold()`不仅仅是用来加数字的。

```rust
fn main() {
    let my_vec = vec![8.0_f64, 7.6, 9.4, 10.0, 22.0, 77.345, 10.22, 3.2, -7.77, -10.0];
    let maximum = my_vec.iter().fold(f64::MIN, |current_number, next_number| current_number.max(*next_number)); // Note: start with the lowest possible number for an f64.
    let minimum = my_vec.iter().fold(f64::MAX, |current_number, next_number| current_number.min(*next_number)); // And here start with the highest possible number
    println!("{}, {}", maximum, minimum);
}
```

### bool

在 Rust 中，如果你愿意，你可以把 `bool` 变成一个整数，因为这样做是安全的。但你不能反过来做。如你所见，`true`变成了1，`false`变成了0。

```rust
fn main() {
    let true_false = (true, false);
    println!("{} {}", true_false.0 as u8, true_false.1 as i32);
}
```

这将打印出`1 0`。如果你告诉编译器类型，也可以使用 `.into()`。

```rust
fn main() {
    let true_false: (i128, u16) = (true.into(), false.into());
    println!("{} {}", true_false.0, true_false.1);
}
```

这打印的是一样的东西。

从Rust 1.50(2021年2月发布)开始，有一个叫做 `then()`的方法，它将一个 `bool`变成一个 `Option`。使用`then()`时需要一个闭包，如果item是`true`，闭包就会被调用。同时，无论从闭包中返回什么，都会进入`Option`中。下面是一个小例子:

```rust
fn main() {

    let (tru, fals) = (true.then(|| 8), false.then(|| 8));
    println!("{:?}, {:?}", tru, fals);
}
```

这个打印 `Some(8), None`。

下面是一个较长的例子:

```rust
fn main() {
    let bool_vec = vec![true, false, true, false, false];

    let option_vec = bool_vec
        .iter()
        .map(|item| {
            item.then(|| { // Put this inside of map so we can pass it on
                println!("Got a {}!", item);
                "It's true, you know" // This goes inside Some if it's true
                                      // Otherwise it just passes on None
            })
        })
        .collect::<Vec<_>>();

    println!("Now we have: {:?}", option_vec);

    // That printed out the Nones too. Let's filter map them out in a new Vec.
    let filtered_vec = option_vec.into_iter().filter_map(|c| c).collect::<Vec<_>>();

    println!("And without the Nones: {:?}", filtered_vec);
}
```

将打印:

```text
Got a true!
Got a true!
Now we have: [Some("It\'s true, you know"), None, Some("It\'s true, you know"), None, None]
And without the Nones: ["It\'s true, you know", "It\'s true, you know"]
```

### Vec

Vec有很多方法我们还没有看。先说说`.sort()`。`.sort()`一点都不奇怪。它使用`&mut self`来对一个向量进行排序。

```rust
fn main() {
    let mut my_vec = vec![100, 90, 80, 0, 0, 0, 0, 0];
    my_vec.sort();
    println!("{:?}", my_vec);
}
```

这样打印出来的是`[0, 0, 0, 0, 0, 80, 90, 100]`。但还有一种更有趣的排序方式叫`.sort_unstable()`，它通常更快。它之所以更快，是因为它不在乎排序前后相同数字的先后顺序。在常规的`.sort()`中，你知道最后的`0, 0, 0, 0, 0`会在`.sort()`之后的顺序相同。但是`.sort_unstable()`可能会把最后一个0移到索引0，然后把第三个最后的0移到索引2，等等。


`.dedup()`的意思是 "去重复"。它将删除一个向量中相同的元素，但只有当它们彼此相邻时才会删除。接下来这段代码不会只打印`"sun", "moon"`。

```rust
fn main() {
    let mut my_vec = vec!["sun", "sun", "moon", "moon", "sun", "moon", "moon"];
    my_vec.dedup();
    println!("{:?}", my_vec);
}
```


它只是把另一个 "sun"旁边的 "sun"去掉，然后把一个 "moon"旁边的 "moon"去掉，再把另一个 "moon"旁边的 "moon"去掉。结果是 `["sun", "moon", "sun", "moon"]`.

如果你想把每个重复的东西都去掉，就先`.sort()`:

```rust
fn main() {
    let mut my_vec = vec!["sun", "sun", "moon", "moon", "sun", "moon", "moon"];
    my_vec.sort();
    my_vec.dedup();
    println!("{:?}", my_vec);
}
```

结果:`["moon", "sun"]`.


### String

你会记得，`String`有点像`Vec`。它很像`Vec`，你可以调用很多相同的方法。比如说，你可以用`String::with_capacity()`创建一个，如果你需要多次用`.push()`推一个`char`，或者用`.push_str()`推一个`&str`。下面是一个有多次内存分配的`String`的例子。

```rust
fn main() {
    let mut push_string = String::new();
    let mut capacity_counter = 0; // capacity starts at 0
    for _ in 0..100_000 { // Do this 100,000 times
        if push_string.capacity() != capacity_counter { // First check if capacity is different now
            println!("{}", push_string.capacity()); // If it is, print it
            capacity_counter = push_string.capacity(); // then update the counter
        }
        push_string.push_str("I'm getting pushed into the string!"); // and push this in every time
    }
}
```

这个打印:

```text
35
70
140
280
560
1120
2240
4480
8960
17920
35840
71680
143360
286720
573440
1146880
2293760
4587520
```

我们不得不重新分配(把所有东西复制过来)18次。但既然我们知道了最终的容量，我们可以马上设置容量，不需要重新分配:只设置一次`String`容量就够了。

```rust
fn main() {
    let mut push_string = String::with_capacity(4587520); // We know the exact number. Some different big number could work too
    let mut capacity_counter = 0;
    for _ in 0..100_000 {
        if push_string.capacity() != capacity_counter {
            println!("{}", push_string.capacity());
            capacity_counter = push_string.capacity();
        }
        push_string.push_str("I'm getting pushed into the string!");
    }
}
```

而这个打印`4587520`。完美的! 我们再也不用分配了。

当然，实际长度肯定比这个小。如果你试了100001次，101000次等等，还是会说`4587520`。这是因为每次的容量都是之前的2倍。不过我们可以用`.shrink_to_fit()`来缩小它(和`Vec`一样)。我们的`String`已经非常大了，我们不想再给它增加任何东西，所以我们可以把它缩小一点。但是只有在你有把握的情况下才可以这样做:下面是原因。

```rust
fn main() {
    let mut push_string = String::with_capacity(4587520);
    let mut capacity_counter = 0;
    for _ in 0..100_000 {
        if push_string.capacity() != capacity_counter {
            println!("{}", push_string.capacity());
            capacity_counter = push_string.capacity();
        }
        push_string.push_str("I'm getting pushed into the string!");
    }
    push_string.shrink_to_fit();
    println!("{}", push_string.capacity());
    push_string.push('a');
    println!("{}", push_string.capacity());
    push_string.shrink_to_fit();
    println!("{}", push_string.capacity());
}
```

这个打印:

```text
4587520
3500000
7000000
3500001
```

所以首先我们的大小是`4587520`，但我们没有全部使用。我们用了`.shrink_to_fit()`，然后把大小降到了`3500000`。但是我们忘记了我们需要推上一个 `a`。当我们这样做的时候，Rust 看到我们需要更多的空间，给了我们双倍的空间:现在是 `7000000`。Whoops! 所以我们又调用了`.shrink_to_fit()`，现在又回到了`3500001`。

`.pop()`对`String`有用，就像对`Vec`一样。

```rust
fn main() {
    let mut my_string = String::from(".daer ot drah tib elttil a si gnirts sihT");
    loop {
        let pop_result = my_string.pop();
        match pop_result {
            Some(character) => print!("{}", character),
            None => break,
        }
    }
}
```

这打印的是`This string is a little bit hard to read.`，因为它是从最后一个字符开始的。

`.retain()`是一个使用闭包的方法，这对`String`来说是罕见的。就像在迭代器上的`.filter()`一样。

```rust
fn main() {
    let mut my_string = String::from("Age: 20 Height: 194 Weight: 80");
    my_string.retain(|character| character.is_alphabetic() || character == ' '); // Keep if a letter or a space
    dbg!(my_string); // Let's use dbg!() for fun this time instead of println!
}
```

这个打印:

```text
[src\main.rs:4] my_string = "Age  Height  Weight "
```


### OsString和CString

`std::ffi`是`std`的一部分，它帮助你将Rust与其他语言或操作系统一起使用。它有`OsString`和`CString`这样的类型，它们就像操作系统的`String`或语言C的`String`一样，它们各自也有自己的`&str`类型:`OsStr`和`CStr`。`ffi`的意思是 "foreign function interface"(外部函数接口)。

当你必须与一个没有Unicode的操作系统一起工作时，你可以使用`OsString`。所有的Rust字符串都是unicode，但不是每个操作系统支持。下面是标准库中关于为什么我们有`OsString`的简单英文解释。

- Unix系统(Linux等)上的字符串可能是很多没有0的字节组合在一起。而且有时你会把它们读成Unicode UTF-8。
- Windows上的字符串可能是由随机的16位值组成的，没有0。有时你会把它们读成Unicode UTF-16。
- 在Rust中，字符串总是有效的UTF-8，其中可能包含0。

所以，`OsString`被设计为支持它们读取。

你可以用一个`OsString`做所有常规的事情，比如`OsString::from("Write something here")`。它还有一个有趣的方法，叫做 `.into_string()`，试图把自己变成一个常规的 `String`。它返回一个 `Result`，但 `Err` 部分只是原来的 `OsString`。

```rust
// 🚧
pub fn into_string(self) -> Result<String, OsString>
```

所以如果不行的话，那你就把它找回来。你不能调用`.unwrap()`，因为它会崩溃，但是你可以使用`match`来找回`OsString`。我们通过调用不存在的方法来测试一下。

```rust
use std::ffi::OsString;

fn main() {
    // ⚠️
    let os_string = OsString::from("This string works for your OS too.");
    match os_string.into_string() {
        Ok(valid) => valid.thth(),           // Compiler: "What's .thth()??"
        Err(not_valid) => not_valid.occg(),  // Compiler: "What's .occg()??"
    }
}
```

然后编译器准确地告诉我们我们想知道的东西。

```text
error[E0599]: no method named `thth` found for struct `std::string::String` in the current scope
 --> src/main.rs:6:28
  |
6 |         Ok(valid) => valid.thth(),
  |                            ^^^^ method not found in `std::string::String`

error[E0599]: no method named `occg` found for struct `std::ffi::OsString` in the current scope
 --> src/main.rs:7:37
  |
7 |         Err(not_valid) => not_valid.occg(),
  |                                     ^^^^ method not found in `std::ffi::OsString`
```

我们可以看到，`valid`的类型是`String`，`not_valid`的类型是`OsString`。

### Mem

`std::mem`有一些非常有趣的方法。我们已经看到了一些，比如`.size_of()`、`.size_of_val()`和`.drop()`。


```rust
use std::mem;

fn main() {
    println!("{}", mem::size_of::<i32>());
    let my_array = [8; 50];
    println!("{}", mem::size_of_val(&my_array));
    let mut some_string = String::from("You can drop a String because it's on the heap");
    mem::drop(some_string);
    // some_string.clear();   If we did this it would panic
}
```

这个打印:

```text
4
200
```

下面是`mem`中的一些其他方法。

`swap()`: 用这个方法你可以交换两个变量之间的值。你可以通过为每个变量创建一个可变引用来做。当你有两个东西想交换，而Rust因为借用规则不让你交换时，这很有帮助。或者只是当你想快速切换两个东西的时候。

这里有一个例子。

```rust
use std::{mem, fmt};

struct Ring { // Create a ring from Lord of the Rings
    owner: String,
    former_owner: String,
    seeker: String, // seeker means "person looking for it"
}

impl Ring {
    fn new(owner: &str, former_owner: &str, seeker: &str) -> Self {
        Self {
            owner: owner.to_string(),
            former_owner: former_owner.to_string(),
            seeker: seeker.to_string(),
        }
    }
}

impl fmt::Display for Ring { // Display to show who has it and who wants it
        fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
            write!(f, "{} has the ring, {} used to have it, and {} wants it", self.owner, self.former_owner, self.seeker)
        }
}

fn main() {
    let mut one_ring = Ring::new("Frodo", "Gollum", "Sauron");
    println!("{}", one_ring);
    mem::swap(&mut one_ring.owner, &mut one_ring.former_owner); // Gollum got the ring back for a second
    println!("{}", one_ring);
}
```

这将打印:

```text
Frodo has the ring, Gollum used to have it, and Sauron wants it
Gollum has the ring, Frodo used to have it, and Sauron wants it
```

`replace()`:这个就像swap一样，其实里面也用了swap，你可以看到。

```rust
pub fn replace<T>(dest: &mut T, mut src: T) -> T {
    swap(dest, &mut src);
    src
}
```

所以它只是做了一个交换，然后返回另一个元素。有了这个，你就用你放进去的其他东西来替换这个值。因为它返回的是旧的值，所以你应该用`let`来使用它。下面是一个简单的例子。

```rust
use std::mem;

struct City {
    name: String,
}

impl City {
    fn change_name(&mut self, name: &str) {
        let old_name = mem::replace(&mut self.name, name.to_string());
        println!(
            "The city once called {} is now called {}.",
            old_name, self.name
        );
    }
}

fn main() {
    let mut capital_city = City {
        name: "Constantinople".to_string(),
    };
    capital_city.change_name("Istanbul");
}
```

这样就会打印出`The city once called Constantinople is now called Istanbul.`。

有一个函数叫`.take()`，和`.replace()`一样，但它在元素中留下了默认值。
 你会记得，默认值通常是0、""之类的东西。这里是签名。

```rust
// 🚧
pub fn take<T>(dest: &mut T) -> T
where
    T: Default,
```

所以你可以做这样的事情。

```rust
use std::mem;

fn main() {
    let mut number_vec = vec![8, 7, 0, 2, 49, 9999];
    let mut new_vec = vec![];

    number_vec.iter_mut().for_each(|number| {
        let taker = mem::take(number);
        new_vec.push(taker);
    });

    println!("{:?}\n{:?}", number_vec, new_vec);
}
```

你可以看到，它将所有数字都替换为0:没有删除任何索引。

```text
[0, 0, 0, 0, 0, 0]
[8, 7, 0, 2, 49, 9999]
```


当然，对于你自己的类型，你可以把`Default`实现成任何你想要的类型。我们来看一个例子，我们有一个`Bank`和一个`Robber`。每次他抢了`Bank`，他就会在桌子上拿到钱。但是办公桌可以随时从后面拿钱，所以它永远有50。我们将为此自制一个类型，所以它将永远有50。下面是它的工作原理。

```rust
use std::mem;
use std::ops::{Deref, DerefMut}; // We will use this to get the power of u32

struct Bank {
    money_inside: u32,
    money_at_desk: DeskMoney, // This is our "smart pointer" type. It has its own default, but it will use u32
}

struct DeskMoney(u32);

impl Default for DeskMoney {
    fn default() -> Self {
        Self(50) // default is always 50, not 0
    }
}

impl Deref for DeskMoney { // With this we can access the u32 using *
    type Target = u32;

    fn deref(&self) -> &Self::Target {
        &self.0
    }
}

impl DerefMut for DeskMoney { // And with this we can add, subtract, etc.
    fn deref_mut(&mut self) -> &mut Self::Target {
        &mut self.0
    }
}

impl Bank {
    fn check_money(&self) {
        println!(
            "There is ${} in the back and ${} at the desk.\n",
            self.money_inside, *self.money_at_desk // Use * so we can just print the u32
        );
    }
}

struct Robber {
    money_in_pocket: u32,
}

impl Robber {
    fn check_money(&self) {
        println!("The robber has ${} right now.\n", self.money_in_pocket);
    }

    fn rob_bank(&mut self, bank: &mut Bank) {
        let new_money = mem::take(&mut bank.money_at_desk); // Here it takes the money, and leaves 50 because that is the default
        self.money_in_pocket += *new_money; // Use * because we can only add u32. DeskMoney can't add
        bank.money_inside -= *new_money;    // Same here
        println!("She robbed the bank. She now has ${}!\n", self.money_in_pocket);
    }
}

fn main() {
    let mut bank_of_klezkavania = Bank { // Set up our bank
        money_inside: 5000,
        money_at_desk: DeskMoney(50),
    };
    bank_of_klezkavania.check_money();

    let mut robber = Robber { // Set up our robber
        money_in_pocket: 50,
    };
    robber.check_money();

    robber.rob_bank(&mut bank_of_klezkavania); // Rob, then check money
    robber.check_money();
    bank_of_klezkavania.check_money();

    robber.rob_bank(&mut bank_of_klezkavania); // Do it again
    robber.check_money();
    bank_of_klezkavania.check_money();

}
```

这将打印:

```text
There is $5000 in the back and $50 at the desk.

The robber has $50 right now.

She robbed the bank. She now has $100!

The robber has $100 right now.

There is $4950 in the back and $50 at the desk.

She robbed the bank. She now has $150!

The robber has $150 right now.

There is $4900 in the back and $50 at the desk.
```

你可以看到桌子上总是有50美元。


### Prelude

标准库也有一个prelude，这就是为什么你不用写`use std::vec::Vec`这样的东西来创建一个`Vec`。你可以[在这里](https://doc.rust-lang.org/std/prelude/index.html#prelude-contents)看到所有这些元素，并且大致了解:

- `std::marker::{Copy, Send, Sized, Sync, Unpin}`. 你以前没有见过`Unpin`，因为几乎每一种类型都会用到它(比如`Sized`，也很常见)。"Pin"的意思是不让东西动。在这种情况下，`Pin`意味着它在内存中不能移动，但大多数元素都有`Unpin`，所以你可以移动。这就是为什么像`std::mem::replace`这样的函数能用，因为它们没有被钉住。
- `std::ops::{Drop, Fn, FnMut, FnOnce}`.
- `std::mem::drop`
- `std::boxed::Box`.
- `std::borrow::ToOwned`. 你之前用`Cow`看到过一点，它可以把借来的内容变成自己的。它使用`.to_owned()`来实现这个功能。你也可以在`&str`上使用`.to_owned()`，得到一个`String`，对于其他借来的值也是一样。
- `std::clone::Clone`
- `std::cmp::{PartialEq, PartialOrd, Eq, Ord}`.
- `std::convert::{AsRef, AsMut, Into, From}`.
- `std::default::Default`.
- `std::iter::{Iterator, Extend, IntoIterator, DoubleEndedIterator, ExactSizeIterator}`. 我们之前用`.rev()`来做迭代器:这实际上是做了一个`DoubleEndedIterator`。`ExactSizeIterator`只是类似于`0..10`的东西:它已经知道自己的`.len()`是10。其他迭代器不知道它们的长度是肯定的。
- `std::option::Option::{self, Some, None}`.
- `std::result::Result::{self, Ok, Err}`.
- `std::string::{String, ToString}`.
- `std::vec::Vec`.

如果你因为某些原因不想要这个prelude怎么办？就加属性`#![no_implicit_prelude]`。我们来试一试，看编译器的抱怨。

```rust
// ⚠️
#![no_implicit_prelude]
fn main() {
    let my_vec = vec![8, 9, 10];
    let my_string = String::from("This won't work");
    println!("{:?}, {}", my_vec, my_string);
}
```

现在Rust根本不知道你想做什么。

```text
error: cannot find macro `println` in this scope
 --> src/main.rs:5:5
  |
5 |     println!("{:?}, {}", my_vec, my_string);
  |     ^^^^^^^

error: cannot find macro `vec` in this scope
 --> src/main.rs:3:18
  |
3 |     let my_vec = vec![8, 9, 10];
  |                  ^^^

error[E0433]: failed to resolve: use of undeclared type or module `String`
 --> src/main.rs:4:21
  |
4 |     let my_string = String::from("This won't work");
  |                     ^^^^^^ use of undeclared type or module `String`

error: aborting due to 3 previous errors
```

因此，对于这个简单的代码，你需要告诉Rust使用`extern`(外部)crate，叫做`std`，然后是你想要的元素。这里是我们要做的一切，只是为了创建一个Vec和一个String，并打印它。

```rust
#![no_implicit_prelude]

extern crate std; // Now you have to tell Rust that you want to use a crate called std
use std::vec; // We need the vec macro
use std::string::String; // and string
use std::convert::From; // and this to convert from a &str to the String
use std::println; // and this to print

fn main() {
    let my_vec = vec![8, 9, 10];
    let my_string = String::from("This won't work");
    println!("{:?}, {}", my_vec, my_string);
}
```

现在终于成功了，打印出`[8, 9, 10], This won't work`。所以你可以明白为什么Rust要用prelude了。但如果你愿意，你不需要使用它。而且你甚至可以使用`#![no_std]`(我们曾经看到过)，用于你连堆栈内存这种东西都用不上的时候。但大多数时候，你根本不用考虑不用prelude或`std`。

那么为什么之前我们没有看到`extern`这个关键字呢？是因为你已经不需要它了。以前，当带入外部crate时，你必须使用它。所以以前要使用`rand`，你必须要写成:

```rust
extern crate rand;
```

然后用 `use` 语句来表示你想使用的修改、trait等。但现在Rust编译器已经不需要这些帮助了--你只需要使用`use`，rust就知道在哪里可以找到它。所以你几乎再也不需要`extern crate`了，但在其他人的Rust代码中，你可能仍然会在顶部看到它。



### Time

`std::time`是你可以找到时间函数的地方。(如果你想要更多的功能，`chrono`这样的crate也可以。)最简单的功能就是用`Instant::now()`获取系统时间即可。

```rust
use std::time::Instant;

fn main() {
    let time = Instant::now();
    println!("{:?}", time);
}
```

如果你打印出来，你会得到这样的东西。`Instant { tv_sec: 2738771, tv_nsec: 685628140 }`. 这说的是秒和纳秒，但用处不大。比如你看2738771秒(写于8月)，就是31.70天。这和月份、日子没有任何关系。但是`Instant`的页面告诉我们，它本身不应该有用。它说它是 "不透明的，只有和Duration一起才有用"。Opaque的意思是 "你搞不清楚"，而Duration的意思是 "过了多少时间"。所以它只有在做比较时间这样的事情时才有用。

如果你看左边的trait，其中一个是`Sub<Instant>`。也就是说我们可以用`-`来减去一个。而当我们点击[src]看它的作用时，页面显示：

```rust
impl Sub<Instant> for Instant {
    type Output = Duration;

    fn sub(self, other: Instant) -> Duration {
        self.duration_since(other)
    }
}
```

因此，它需要一个`Instant`，并使用`.duration_since()`给出一个`Duration`。让我们试着打印一下。我们将创建两个相邻的 `Instant::now()`，然后让程序忙活一会儿，再创建一个 `Instant::now()`。然后我们再创建一个`Instant::now()`. 最后，我们来看看用了多长时间。

```rust
use std::time::Instant;

fn main() {
    let time1 = Instant::now();
    let time2 = Instant::now(); // These two are right next to each other

    let mut new_string = String::new();
    loop {
        new_string.push('წ'); // Make Rust push this Georgian letter onto the String
        if new_string.len() > 100_000 { //  until it is 100,000 bytes long
            break;
        }
    }
    let time3 = Instant::now();
    println!("{:?}", time2 - time1);
    println!("{:?}", time3 - time1);
}
```

这将打印出这样的东西。

```text
1.025µs
683.378µs
```

所以，这只是1微秒多与683毫秒。我们可以看到，Rust确实花了一些时间来做。

不过我们可以用一个`Instant`做一件有趣的事情。
 我们可以把它变成`String`与`format!("{:?}", Instant::now());`。它的样子是这样的:

```rust
use std::time::Instant;

fn main() {
    let time1 = format!("{:?}", Instant::now());
    println!("{}", time1);
}
```

这样就会打印出类似`Instant { tv_sec: 2740773, tv_nsec: 632821036 }`的东西。这是没有用的，但是如果我们使用 `.iter()` 和 `.rev()` 以及 `.skip(2)`，我们可以跳过最后的 `}` 和 ` `。我们可以用它来创建一个随机数发生器。

```rust
use std::time::Instant;

fn bad_random_number(digits: usize) {
    if digits > 9 {
        panic!("Random number can only be up to 9 digits");
    }
    let now = Instant::now();
    let output = format!("{:?}", now);

    output
        .chars()
        .rev()
        .skip(2)
        .take(digits)
        .for_each(|character| print!("{}", character));
    println!();
}

fn main() {
    bad_random_number(1);
    bad_random_number(1);
    bad_random_number(3);
    bad_random_number(3);
}
```

这样就会打印出类似这样的内容:

```text
6
4
967
180
```

这个函数被称为`bad_random_number`，因为它不是一个很好的随机数生成器。Rust有更好的crate，可以用比`rand`更少的代码创建随机数，比如`fastrand`。但这是一个很好的例子，你可以利用你的想象力用`Instant`来做一些事情。

当你有一个线程时，你可以使用`std::thread::sleep`使它停止一段时间。当你这样做时，你必须给它一个duration。你不必创建多个线程来做这件事，因为每个程序至少在一个线程上。`sleep`虽然需要一个`Duration`，所以它可以知道要睡多久。你可以这样选单位:`Duration::from_millis()`, `Duration::from_secs`, 等等。这里举一个例子:

```rust
use std::time::Duration;
use std::thread::sleep;

fn main() {
    let three_seconds = Duration::from_secs(3);
    println!("I must sleep now.");
    sleep(three_seconds);
    println!("Did I miss anything?");
}
```

这将只打印

```text
I must sleep now.
Did I miss anything?
```

但线程在三秒钟内什么也不做。当你有很多线程需要经常尝试一些事情时，比如连接，你通常会使用`.sleep()`。你不希望线程在一秒钟内使用你的处理器尝试10万次，而你只是想让它有时检查一下。所以，你就可以设置一个`Duration`，它就会在每次醒来的时候尝试做它的任务。


### 其他宏


我们再来看看其他一些宏。

`unreachable!()`

这个宏有点像`todo!()`，除了它是针对你永远不会用的代码。也许你在一个枚举中有一个`match`，你知道它永远不会选择其中的一个分支，所以代码永远无法达到那个分支。如果是这样，你可以写`unreachable!()`，这样编译器就知道可以忽略这部分。

例如，假设你有一个程序，当你选择一个地方居住时，它会写一些东西。在乌克兰，除了切尔诺贝利，其他地方都不错。你的程序不让任何人选择切尔诺贝利，因为它现在不是一个好地方。但是这个枚举是很早以前在别人的代码里做的，你无法更改。所以在`match`的分支中，你可以用这个宏。它是这样的:

```rust
enum UkrainePlaces {
    Kiev,
    Kharkiv,
    Chernobyl, // Pretend we can't change the enum - Chernobyl will always be here
    Odesa,
    Dnipro,
}

fn choose_city(place: &UkrainePlaces) {
    use UkrainePlaces::*;
    match place {
        Kiev => println!("You will live in Kiev"),
        Kharkiv => println!("You will live in Kharkiv"),
        Chernobyl => unreachable!(),
        Odesa => println!("You will live in Odesa"),
        Dnipro => println!("You will live in Dnipro"),
    }
}

fn main() {
    let user_input = UkrainePlaces::Kiev; // Pretend the user input is made from some other function. The user can't choose Chernobyl, no matter what
    choose_city(&user_input);
}
```

这将打印出 `You will live in Kiev`。

`unreachable!()`对你来说也很好读，因为它提醒你代码的某些部分是不可访问的。不过你必须确定代码确实是不可访问的。如果编译器调用`unreachable!()`，程序就会崩溃。

此外，如果你曾经有不可达的代码，而编译器知道，它会告诉你。下面是一个简单的例子:

```rust
fn main() {
    let true_or_false = true;

    match true_or_false {
        true => println!("It's true"),
        false => println!("It's false"),
        true => println!("It's true"), // Whoops, we wrote true again
    }
}
```

它会说

```text
warning: unreachable pattern
 --> src/main.rs:7:9
  |
7 |         true => println!("It's true"),
  |         ^^^^
  |
```

但是`unreachable!()`是用于编译器无法知道的时候，就像我们另一个例子。



`column!`, `line!`, `file!`, `module_path!`

这四个宏有点像`dbg!()`，因为你只是把它们放进代码去给你调试信息。但是它们不需要任何变量--你只需要用它们和括号一起使用，而没有其他的东西。它们放到一起很容易学:

- `column!()`给你写的那一列
- `file!()`给你写的文件的名称
- `line!()`给你写的那行字，然后是
- `module_path!()`给你模块的位置。

接下来的代码在一个简单的例子中展示了这三者。我们将假装有更多的代码(mod里面的mod)，因为这就是我们要使用这些宏的原因。你可以想象一个大的Rust程序,它有许多mod和文件。

```rust
pub mod something {
    pub mod third_mod {
        pub fn print_a_country(input: &mut Vec<&str>) {
            println!(
                "The last country is {} inside the module {}",
                input.pop().unwrap(),
                module_path!()
            );
        }
    }
}

fn main() {
    use something::third_mod::*;
    let mut country_vec = vec!["Portugal", "Czechia", "Finland"];

    // do some stuff
    println!("Hello from file {}", file!());

    // do some stuff
    println!(
        "On line {} we got the country {}",
        line!(),
        country_vec.pop().unwrap()
    );

    // do some more stuff

    println!(
        "The next country is {} on line {} and column {}.",
        country_vec.pop().unwrap(),
        line!(),
        column!(),
    );

    // lots more code

    print_a_country(&mut country_vec);
}
```

它打印的是这样的。

```text
Hello from file src/main.rs
On line 23 we got the country Finland
The next country is Czechia on line 32 and column 9.
The last country is Portugal inside the module rust_book::something::third_mod
```



`cfg!`

我们知道，你可以使用 `#[cfg(test)]` 和 `#[cfg(windows)]` 这样的属性来告诉编译器在某些情况下该怎么做。当你有`test`时，当你在测试模式下运行Rust时，它会运行代码(如果是在电脑上，你输入`cargo test`)。而当你使用`windows`时，如果用户使用的是Windows，它就会运行代码。但也许你只是想根据不同操作系统对依赖系统的代码做很小的修改。这时候这个宏就很有用了。它返回一个`bool`。

```rust
fn main() {
    let helpful_message = if cfg!(target_os = "windows") { "backslash" } else { "slash" };

    println!(
        "...then in your hard drive, type the directory name followed by a {}. Then you...",
        helpful_message
    );
}
```

这将以不同的方式打印，取决于你的系统。Rust Playground在Linux上运行，所以会打印:

```text
...then in your hard drive, type the directory name followed by a slash. Then you...
```

`cfg!()`适用于任何一种配置。下面是一个例子，当你在测试中使用一个函数时，它的运行方式会有所不同。

```rust
#[cfg(test)] // cfg! will know to look for the word test
mod testing {
    use super::*;
    #[test]
    fn check_if_five() {
        assert_eq!(bring_number(true), 5); // This bring_number() function should return 5
    }
}

fn bring_number(should_run: bool) -> u32 { // This function takes a bool as to whether it should run
    if cfg!(test) && should_run { // if it should run and has the configuration test, return 5
        5
    } else if should_run { // if it's not a test but it should run, print something. When you run a test it ignores println! statements
        println!("Returning 5. This is not a test");
        5
    } else {
        println!("This shouldn't run, returning 0."); // otherwise return 0
        0
    }
}

fn main() {
    bring_number(true);
    bring_number(false);
}
```

现在根据配置的不同，它的运行方式也会不同。如果你只是运行程序，它会给你这样的结果:

```text
Returning 5. This is not a test
This shouldn't run, returning 0.
```

但如果你在测试模式下运行它(`cargo test`，用于电脑上的Rust)，它实际上会运行测试。因为在这种情况下，测试总是返回5，所以它会通过。

```text
running 1 test
test testing::check_if_five ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out
```



## 编写宏

编写宏是非常复杂的。你可能永远都不需要写宏，但有时你可能会想写，因为它们非常方便。写宏很有趣，因为它们几乎是不同的语言。要写一个宏，你实际上是用另一个叫`macro_rules!`的宏。然后你添加你的宏名称，并打开一个`{}`块。里面有点像`match`语句。

这里有一个只取`()`，然后返回6:

```rust
macro_rules! give_six {
    () => {
        6
    };
}

fn main() {
    let six = give_six!();
    println!("{}", six);
}
```

但这和`match`语句是不一样的，因为宏实际上不会编译任何东西。它只是接受一个输入并给出一个输出。然后编译器会检查它是否有意义。这就是为什么宏就像 "写代码的代码"。你会记得，一个真正的`match`语句需要给出相同的类型，所以这不会工作:

```rust
fn main() {
// ⚠️
    let my_number = 10;
    match my_number {
        10 => println!("You got a ten"),
        _ => 10,
    }
}
```

它会抱怨你在一种情况下要返回`()`，在另一种情况下要返回`i32`。

```text
error[E0308]: `match` arms have incompatible types
 --> src\main.rs:5:14
  |
3 | /     match my_number {
4 | |         10 => println!("You got a ten"),
  | |               ------------------------- this is found to be of type `()`
5 | |         _ => 10,
  | |              ^^ expected `()`, found integer
6 | |     }
  | |_____- `match` arms have incompatible types
```

但宏并不关心，因为它只是给出一个输出。它不是一个编译器--它是代码前的代码。所以你可以这样做:

```rust
macro_rules! six_or_print {
    (6) => {
        6
    };
    () => {
        println!("You didn't give me 6.");
    };
}

fn main() {
    let my_number = six_or_print!(6);
    six_or_print!();
}
```

这个就好办了，打印的是`You didn't give me 6.`。你也可以看到，这不是匹配分支，因为没有`_`行。我们只能给它`(6)`，或者`()`，其他的都会出错。而我们给它的`6`甚至不是`i32`，只是一个输入6。其实你可以设置任何东西作为宏的输入，因为它只是看输入，看得到什么。比如说:

```rust
macro_rules! might_print {
    (THis is strange input 하하はは哈哈 but it still works) => {
        println!("You guessed the secret message!")
    };
    () => {
        println!("You didn't guess it");
    };
}

fn main() {
    might_print!(THis is strange input 하하はは哈哈 but it still works);
    might_print!();
}
```

所以这个奇怪的宏只响应两件事。`()`和`(THis is strange input 하하はは哈哈 but it still works)`. 没有其他的东西。它打印的是:

```text
You guessed the secret message!
You didn't guess it
```

所以宏不完全是Rust语法。但是宏也可以理解你给它的不同类型的输入。拿这个例子来说。

```rust
macro_rules! might_print {
    ($input:expr) => {
        println!("You gave me: {}", $input);
    }
}

fn main() {
    might_print!(6);
}
```

这将打印`You gave me: 6`。`$input:expr`部分很重要。它的意思是 "对于一个表达式，给它起一个变量名$input"。在宏中，变量以`$`开头。在这个宏中，如果你给它一个表达式，它就会打印出来。我们再来试一试。

```rust
macro_rules! might_print {
    ($input:expr) => {
        println!("You gave me: {:?}", $input); // Now we'll use {:?} because we will give it different kinds of expressions
    }
}

fn main() {
    might_print!(()); // give it a ()
    might_print!(6); // give it a 6
    might_print!(vec![8, 9, 7, 10]); // give it a vec
}
```

这将打印:

```text
You gave me: ()
You gave me: 6
You gave me: [8, 9, 7, 10]
```

另外注意，我们写了`{:?}`，但它不会检查`&input`是否实现了`Debug`。它只会写代码，并尝试让它编译，如果没有，那么它就会给出一个错误。

那么除了`expr`，宏还能看到什么呢？它们是 `block | expr | ident | item | lifetime | literal  | meta | pat | path | stmt | tt | ty | vis`. 这就是复杂的部分。你可以在[这里](https://doc.rust-lang.org/beta/reference/macros-by-example.html)看到它们各自的意思，这里说:

```text
item: an Item
block: a BlockExpression
stmt: a Statement without the trailing semicolon (except for item statements that require semicolons)
pat: a Pattern
expr: an Expression
ty: a Type
ident: an IDENTIFIER_OR_KEYWORD
path: a TypePath style path
tt: a TokenTree (a single token or tokens in matching delimiters (), [], or {})
meta: an Attr, the contents of an attribute
lifetime: a LIFETIME_TOKEN
vis: a possibly empty Visibility qualifier
literal: matches -?LiteralExpression
```

另外有一个很好的网站叫cheats.rs，在[这里](https://cheats.rs/#macros-attributes)解释了它们，并且每个都给出了例子。

然而，对于大多数宏，你只会用到 `expr`、`ident` 和 `tt`。`ident` 表示标识符，用于变量或函数名称。`tt`表示token树，和任何类型的输入。让我们尝试用这两个词创建一个简单的宏。

```rust
macro_rules! check {
    ($input1:ident, $input2:expr) => {
        println!(
            "Is {:?} equal to {:?}? {:?}",
            $input1,
            $input2,
            $input1 == $input2
        );
    };
}

fn main() {
    let x = 6;
    let my_vec = vec![7, 8, 9];
    check!(x, 6);
    check!(my_vec, vec![7, 8, 9]);
    check!(x, 10);
}
```

所以这将取一个`ident`(像一个变量名)和一个表达式，看看它们是否相同。它的打印结果是

```text
Is 6 equal to 6? true
Is [7, 8, 9] equal to [7, 8, 9]? true
Is 6 equal to 10? false
```

而这里有一个宏，输入`tt`，然后把它打印出来。它先用一个叫`stringify!`的宏创建一个字符串。

```rust
macro_rules! print_anything {
    ($input:tt) => {
        let output = stringify!($input);
        println!("{}", output);
    };
}

fn main() {
    print_anything!(ththdoetd);
    print_anything!(87575oehq75onth);
}
```

这个将打印:

```text
ththdoetd
87575oehq75onth
```

但是如果我们给它一些带有空格、逗号等的东西，它就不会打印。它会认为我们给了它不止一个元素或额外的信息，所以它会感到困惑。

这就是宏开始变得困难的地方。

要一次给宏提供多个元素，我们必须使用不同的语法。不要用`$input`，而是`$($input1),*`。这意味着零或更多(这是 * 的意思)，用逗号分隔。如果你想要一个或多个，请使用 `+` 而不是 `*`。

现在我们的宏看起来是这样的。

```rust
macro_rules! print_anything {
    ($($input1:tt),*) => {
        let output = stringify!($($input1),*);
        println!("{}", output);
    };
}


fn main() {
    print_anything!(ththdoetd, rcofe);
    print_anything!();
    print_anything!(87575oehq75onth, ntohe, 987987o, 097);
}
```

所以它接受任何用逗号隔开的token树，并使用 `stringify!` 把它变成一个字符串。然后打印出来。它的打印结果是:

```text
ththdoetd, rcofe

87575oehq75onth, ntohe, 987987o, 097
```

如果我们使用`+`而不是`*`，它会给出一个错误，因为有一次我们没有给它输入。所以`*`是一个比较安全的选择。

所以现在我们可以开始看到宏的威力了。在接下来的这个例子中，我们实际上可以创建我们自己的函数:

```rust
macro_rules! make_a_function {
    ($name:ident, $($input:tt),*) => { // First you give it one name for the function, then it checks everything else
        fn $name() {
            let output = stringify!($($input),*); // It makes everything else into a string
            println!("{}", output);
        }
    };
}


fn main() {
    make_a_function!(print_it, 5, 5, 6, I); // We want a function called print_it() that prints everything else we give it
    print_it();
    make_a_function!(say_its_nice, this, is, really, nice); // Same here but we change the function name
    say_its_nice();
}
```

这个打印:

```text
5, 5, 6, I
this, is, really, nice
```


所以现在我们可以开始了解其他的宏了。你可以看到，我们已经使用的一些宏非常简单。这里是我们用来写入文件的`write!`的那个:

```rust
macro_rules! write {
    ($dst:expr, $($arg:tt)*) => ($dst.write_fmt($crate::format_args!($($arg)*)))
}
```

要使用它，你就输入这个:

- 一个表达式(`expr`) 得到变量名`$dst`.
- 之后的一切。如果它写的是`$arg:tt`，那么它只会取1个，但是因为它写的是`$($arg:tt)*`，所以它取0，1，或者任意多个。

然后它取`$dst`，并对它使用了一个叫做`write_fmt`的方法。在这里面，它使用了另一个叫做`format_args!`的宏，它接受所有的`$($arg)*`，或者我们输入的所有参数。



现在我们来看一下`todo!`这个宏。当你想让程序编译但还没有写出你的代码时，就会用到这个宏。它看起来像这样:

```rust
macro_rules! todo {
    () => (panic!("not yet implemented"));
    ($($arg:tt)+) => (panic!("not yet implemented: {}", $crate::format_args!($($arg)+)));
}
```

这个有两个选项:你可以输入`()`，也可以输入一些token树(`tt`)。

- 如果你输入`()`，它只是`panic!`，并加上一个信息。所以其实你可以直接写`panic!("not yet implemented")`，而不是`todo!`，这也是一样的。
- 如果你输入一些参数，它会尝试打印它们。你可以看到里面有同样的`format_args!`宏，它的工作原理和`println!`一样。

所以，如果你写了这个，它也会工作:

```rust
fn not_done() {
    let time = 8;
    let reason = "lack of time";
    todo!("Not done yet because of {}. Check back in {} hours", reason, time);
}

fn main() {
    not_done();
}
```

这将打印:

```text
thread 'main' panicked at 'not yet implemented: Not done yet because of lack of time. Check back in 8 hours', src/main.rs:4:5
```


在一个宏里面，你甚至可以调用同一个宏。这里有一个。

```rust
macro_rules! my_macro {
    () => {
        println!("Let's print this.");
    };
    ($input:expr) => {
        my_macro!();
    };
    ($($input:expr),*) => {
        my_macro!();
    }
}

fn main() {
    my_macro!(vec![8, 9, 0]);
    my_macro!(toheteh);
    my_macro!(8, 7, 0, 10);
    my_macro!();
}
```

这个可以取`()`，也可以取一个表达式，也可以取很多表达式。但是不管你放什么表达式，它都会忽略所有的表达式，只是在`()`上调用`my_macro!`。所以输出的只是`Let's print this`，四次。

在`dbg!`宏中也可以看到同样的情况，也是调用自己。

```rust
macro_rules! dbg {
    () => {
        $crate::eprintln!("[{}:{}]", $crate::file!(), $crate::line!()); //$crate means the crate that it's in.
    };
    ($val:expr) => {
        // Use of `match` here is intentional because it affects the lifetimes
        // of temporaries - https://stackoverflow.com/a/48732525/1063961
        match $val {
            tmp => {
                $crate::eprintln!("[{}:{}] {} = {:#?}",
                    $crate::file!(), $crate::line!(), $crate::stringify!($val), &tmp);
                tmp
            }
        }
    };
    // Trailing comma with single argument is ignored
    ($val:expr,) => { $crate::dbg!($val) };
    ($($val:expr),+ $(,)?) => {
        ($($crate::dbg!($val)),+,)
    };
}
```

(`eprintln!`与`println!`相同，只打印到`io::stderr`而不是`io::stdout`。还有`eprint!`不增加一行)。)

所以我们可以自己去试一试。

```rust
fn main() {
    dbg!();
}
```

这与第一分支相匹配，所以它会用`file!`和`line!`宏打印文件名和行名。它打印的是`[src/main.rs:2]`。

我们用这个来试试。

```rust
fn main() {
    dbg!(vec![8, 9, 10]);
}
```

这将匹配下一个分支，因为它是一个表达式。然后它将调用输入`tmp`并使用这个代码。` $crate::eprintln!("[{}:{}] {} = {:#?}", $crate::file!(), $crate::line!(), $crate::stringify!($val), &tmp);`. 所以它会用`file!`和`line!`来打印，然后把`$val`做成`String`，用`{:#?}`来漂亮的打印`tmp`。所以对于我们的输入，它会这样写。

```text
[src/main.rs:2] vec![8, 9, 10] = [
    8,
    9,
    10,
]
```

剩下的部分，即使你多加了一个逗号，它也只是自己调用`dbg!`。

正如你所看到的，宏是非常复杂的！通常你只想让一个宏自动完成一些简单函数不能很好完成的事情。学习宏的最好方法是看其他宏的例子。没有多少人能够快速写出宏而不出问题。所以不要认为你需要知道宏的一切，才能知道如何在Rust中写。但如果你读了其他宏，并稍加修改，你就可以很容易地借用它们的力量。然后你可能会开始适应写自己的宏。


# 第2部分 - 电脑上的Rust

你看到了，我们几乎可以使用Playground学习Rust中的任何东西。但如果你到目前为止已经学了这么多，现在你可能会想要在你的电脑上使用Rust。总有一些事情是你不能用Playground做的，比如使用文件或代码在多个文件中。其他如输入和flags也需要在电脑上安装Rust。但最重要的是，在你的电脑上有了Rust，你可以使用Crate。我们已经了解了crate，但在playground中你只能使用最流行的crate。但在你的电脑上，你可以在程序中使用任何crate。

## cargo

`rustc`的意思是Rust编译器，实际的编译工作由它完成。一个rust文件的结尾是`.rs`。但大多数人不会写出类似 `rustc main.rs` 的东西来编译。他们使用的是名为 `cargo` 的东西，它是 Rust 的主包管理器。

关于这个名字的一个说明: 之所以叫`cargo`，是因为当你把crate放在一起时，你会得到cargo。Crate就是你在船上或卡车上看到的木箱，但你记住，每个Rust项目也叫Crate。那么当你把它们放在一起时，你就会得到整个cargo。

当你使用cargo来运行一个项目时，你可以看到这一点。让我们用 `rand` 试试简单的东西:我们只是在八个字母之间随机选择。

```rust
use rand::seq::SliceRandom; // Use this for .choose over slices

fn main() {

    let my_letters = vec!['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h'];

    let mut rng = rand::thread_rng();
    for _ in 0..6 {
        print!("{} ", my_letters.choose(&mut rng).unwrap());
    }
}
```

这样就会打印出`b c g h e a`这样的东西。但我们想先看看`cargo`的作用。要使用 `cargo` 并运行我们的程序，通常我们输入 `cargo run`。这样就可以构建我们的程序，并为我们运行它。当它开始编译的时候，会做这样的事情:

```text
   Compiling getrandom v0.1.14
   Compiling cfg-if v0.1.10
   Compiling ppv-lite86 v0.2.8
   Compiling rand_core v0.5.1
   Compiling rand_chacha v0.2.2
   Compiling rand v0.7.3
   Compiling rust_book v0.1.0 (C:\Users\mithr\OneDrive\Documents\Rust\rust_book)
    Finished dev [unoptimized + debuginfo] target(s) in 13.13s
     Running `C:\Users\mithr\OneDrive\Documents\Rust\rust_book\target\debug\rust_book.exe`
g f c f h b
```

所以看起来不只是引入了`rand`，还引入了一些其他的crate。这是因为我们的crate需要`rand`，但`rand`也有一些代码也需要其他crate。所以`cargo`会找到我们需要的所有crate，并把它们放在一起。在我们的案例中，只有7个，但在非常大的项目中，你可能会有200个或更多的crate要引入。

这就是你可以看到Rust的权衡的地方。Rust的速度非常快，因为它提前编译。它通过查看代码，看你写的代码到底做了什么。例如，你可能会写这样的泛型代码:

```rust
use std::fmt::Display;

fn print_and_return_thing<T: Display>(input: T) -> T {
    println!("You gave me {} and now I will give it back.", input);
    input
}

fn main() {
    let my_name = print_and_return_thing("Windy");
    let small_number = print_and_return_thing(9.0);
}
```

这个函数可以用任何实现了`Display`的作为参数，所以我们给它一个`&str`，接下来给它一个`f64`，这对我们来说是没有问题的。但是编译器不看泛型，因为它不想在运行时做任何事情。它想把一个能运行的程序尽可能快地组装起来。所以当它看第一部分的`"Windy"`时，它没有看到`fn print_and_return_thing<T: Display>(input: T) -> T`，它看到的是`fn print_and_return_thing(input: &str) -> &str`这样的东西。而接下来它看到的是`fn print_and_return_thing(input: f64) -> f64`。所有关于trait的检查等等都是在编译时完成的。这就是为什么泛型需要更长的时间来编译，因为它需要弄清楚它们，并使之具体化。

还有一点:Rust 2020正在努力处理编译时间问题，因为这部分需要的时间最长。每一个版本的Rust在编译时都会快一点，而且还有一些其他的计划来加快它的速度。但与此同时，以下是你应该知道的:

- `cargo build`会构建你的程序，这样你就可以运行它了。
- `cargo run`将建立你的程序并运行它。
- `cargo build --release`和`cargo run --release`发布模式下有同样的效果。什么是发布模式？当你的代码最终完成后就可以用发布模式了。Rust会花更多的时间来编译，但它这样做是因为它使用了它所知道的一切，来使编译出的程序运行更快。Release模式实际上比常规模式*快的多*，常规模式被称为debug模式。那是因为它的编译速度更快，而且有更多的调试信息。常规的`cargo build`叫做 "debug build"，`cargo build --release`叫做 "release build"。
- `cargo check`是一种检查代码的方式。它就像编译一样，只不过它不会真正地创建你的程序。这是一个很好的检查你的代码的方法，因为它不像`build`或`run`那样需要很长时间。

对了，命令中的`--release`部分叫做`flag`。这意味着命令中的额外信息。

其他一些你需要知道的事情是:

- `cargo new`. 这样做是为了创建一个新的Rust项目。`new`之后，写上项目的名称，`cargo`将会创建所有你需要的文件和文件夹。
- `cargo clean`. 当你把crate添加到`Cargo.toml`时，电脑会下载所有需要的文件，它们会占用很多空间。如果你不想再让它们在你的电脑上，输入`cargo clean`。

关于编译器还有一点:只有当你第一次使用`cargo build`或`cargo run`时，它才会花费最多的时间。之后它就会记住，它又会快速编译。但如果你使用 `cargo clean`，然后运行 `cargo build`，它将不得不再慢慢地编译一次。


## 接受用户输入

一个简单的方法是用`std::io::stdin`来接受用户的输入。这意味着 "标准输入"，也就是来自键盘的输入。用`stdin()`可以获得用户的输入，但是接下来你就会想用`.read_line()`把它放到`&mut String`中。下面是一个简单的例子，但它既能工作，也不能工作:

```rust
use std::io;

fn main() {
    println!("Please type something, or x to escape:");
    let mut input_string = String::new();

    while input_string != "x" { // This is the part that doesn't work right
        input_string.clear(); // First clear the String. Otherwise it will keep adding to it
        io::stdin().read_line(&mut input_string).unwrap(); // Get the stdin from the user, and put it in read_string
        println!("You wrote {}", input_string);
    }
    println!("See you later!");
}
```

下面是一个输出输出的样子。

```text
Please type something, or x to escape:
something
You wrote something

Something else
You wrote Something else

x
You wrote x

x
You wrote x

x
You wrote x
```

它接受我们的输入，然后把它还给我们，它甚至知道我们输入了`x`。但它并没有退出程序。唯一的办法是关闭窗口，或者输入ctrl和c。让我们把`println!`中的`{}`改为`{:?}`，以获得更多的信息(如果你喜欢那个宏，也可以使用`dbg!(&input_string)`)。现在它说

```text
Please type something, or x to escape:
something
You wrote "something\r\n"
Something else
You wrote "Something else\r\n"
x
You wrote "x\r\n"
x
You wrote "x\r\n"
```



这是因为键盘输入其实不只是`something`，而是`something`和`Enter`键。有一个简单的方法可以解决这个问题，叫做`.trim()`，它可以把所有的空白都去掉。顺便说一下，[这些字符](https://doc.rust-lang.org/reference/whitespace.html)都是空白字符。

```text
U+0009 (horizontal tab, '\t')
U+000A (line feed, '\n')
U+000B (vertical tab)
U+000C (form feed)
U+000D (carriage return, '\r')
U+0020 (space, ' ')
U+0085 (next line)
U+200E (left-to-right mark)
U+200F (right-to-left mark)
U+2028 (line separator)
U+2029 (paragraph separator)
```

这样就可以把`x\r\n`变成只剩`x`了。现在它可以工作了:

```rust
use std::io;

fn main() {
    println!("Please type something, or x to escape:");
    let mut input_string = String::new();

    while input_string.trim() != "x" {
        input_string.clear();
        io::stdin().read_line(&mut input_string).unwrap();
        println!("You wrote {}", input_string);
    }
    println!("See you later!");
}
```

现在可以打印了:

```text
Please type something, or x to escape:
something
You wrote something

Something
You wrote Something

x
You wrote x

See you later!
```



还有一种用户输入叫`std::env::Args`(env是环境的意思)。`Args`是用户启动程序时输入的内容。其实在一个程序中总是至少有一个`Arg`。我们写一个程序，只用`std::env::args()`来打印它们，看看它们是什么。

```rust
fn main() {
    println!("{:?}", std::env::args());
}
```

如果我们写`cargo run`，那么它的打印结果是这样的:

```text
Args { inner: ["target\\debug\\rust_book.exe"] }
```

让我们给它更多的输入，看看它的作用。我们输入 `cargo run but with some extra words` 。 它给我们:

```text
Args { inner: ["target\\debug\\rust_book.exe", "but", "with", "some", "extra", "words"] }
```

有意思。而当我们查看[Args的页面](https://doc.rust-lang.org/std/env/struct.Args.html)时，我们看到它实现了`IntoIterator`。这意味着我们可以.用所有我们知道的关于迭代器的方法来读取和改变它。让我们试试这个:

```rust
use std::env::args;

fn main() {
    let input = args();

    for entry in input {
        println!("You entered: {}", entry);
    }
}
```

现在它说:

```text
You entered: target\debug\rust_book.exe
You entered: but
You entered: with
You entered: some
You entered: extra
You entered: words
```

你可以看到，第一个参数总是程序名，所以你经常会想跳过它，比如这样:

```rust
use std::env::args;

fn main() {
    let input = args();

    input.skip(1).for_each(|item| {
        println!("You wrote {}, which in capital letters is {}", item, item.to_uppercase());
    })
}
```

这将打印:

```text
You wrote but, which in capital letters is BUT
You wrote with, which in capital letters is WITH
You wrote some, which in capital letters is SOME
You wrote extra, which in capital letters is EXTRA
You wrote words, which in capital letters is WORDS
```

`Args`的一个常见用途是用于用户设置。你可以确保用户写出你需要的输入，只有在正确的情况下才运行程序。这里有一个小程序，可以让字母变大(大写)或变小(小写)。

```rust
use std::env::args;

enum Letters {
    Capitalize,
    Lowercase,
    Nothing,
}

fn main() {
    let mut changes = Letters::Nothing;
    let input = args().collect::<Vec<_>>();

    if input.len() > 2 {
        match input[1].as_str() {
            "capital" => changes = Letters::Capitalize,
            "lowercase" => changes = Letters::Lowercase,
            _ => {}
        }
    }

    for word in input.iter().skip(2) {
      match changes {
        Letters::Capitalize => println!("{}", word.to_uppercase()),
        Letters::Lowercase => println!("{}", word.to_lowercase()),
        _ => println!("{}", word)
      }
    }

}
```

下面是它给出的一些例子。

输入: `cargo run please make capitals`:

```text
make capitals
```

输入:`cargo run capital`:

```text
// Nothing here...
```

输入:`cargo run capital I think I understand now`:

```text
I
THINK
I
UNDERSTAND
NOW
```

输入:`cargo run lowercase Does this work too?`

```text
does
this
work
too?
```



除了用户给出的 `Args`，在 `std::env::args()` 中可用，还有系统变量`Vars`。这些都是用户没有输入的程序的基本设置。你可以用`std::env::vars()`把它们都看成一个`(String, String)`。这个有非常多，比如说:

```rust
fn main() {
    for item in std::env::vars() {
        println!("{:?}", item);
    }
}
```

运行这段代码，就能显示出你的用户会话的所有信息。它将显示这样的信息:

```text
("CARGO", "/playground/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/bin/cargo")
("CARGO_HOME", "/playground/.cargo")
("CARGO_MANIFEST_DIR", "/playground")
("CARGO_PKG_AUTHORS", "The Rust Playground")
("CARGO_PKG_DESCRIPTION", "")
("CARGO_PKG_HOMEPAGE", "")
("CARGO_PKG_NAME", "playground")
("CARGO_PKG_REPOSITORY", "")
("CARGO_PKG_VERSION", "0.0.1")
("CARGO_PKG_VERSION_MAJOR", "0")
("CARGO_PKG_VERSION_MINOR", "0")
("CARGO_PKG_VERSION_PATCH", "1")
("CARGO_PKG_VERSION_PRE", "")
("DEBIAN_FRONTEND", "noninteractive")
("HOME", "/playground")
("HOSTNAME", "f94c15b8134b")
("LD_LIBRARY_PATH", "/playground/target/debug/build/backtrace-sys-3ec4c973f371c302/out:/playground/target/debug/build/libsqlite3-sys-fbddfbb9b241dacb/out:/playground/target/debug/build/ring-cadba5e583648abb/out:/playground/target/debug/deps:/playground/target/debug:/playground/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/lib/rustlib/x86_64-unknown-linux-gnu/lib:/playground/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/lib")
("PATH", "/playground/.cargo/bin:/playground/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin")
("PLAYGROUND_EDITION", "2018")
("PLAYGROUND_TIMEOUT", "10")
("PWD", "/playground")
("RUSTUP_HOME", "/playground/.rustup")
("RUSTUP_TOOLCHAIN", "stable-x86_64-unknown-linux-gnu")
("RUST_RECURSION_COUNT", "1")
("SHLVL", "1")
("SSL_CERT_DIR", "/usr/lib/ssl/certs")
("SSL_CERT_FILE", "/usr/lib/ssl/certs/ca-certificates.crt")
("USER", "playground")
("_", "/usr/bin/timeout")
```

所以如果你需要这些信息，`Vars`就是你想要的。

获得单个`Var'的最简单方法是使用`env!`宏。你只要给它变量的名字，它就会给你一个`&str'的值。如果变量拼写错误或不存在，它就不起作用，所以如果你不确定，就用`option_env!`代替。如果我们在Playground上写这个:

```rust
fn main() {
    println!("{}", env!("USER"));
    println!("{}", option_env!("ROOT").unwrap_or("Can't find ROOT"));
    println!("{}", option_env!("CARGO").unwrap_or("Can't find CARGO"));
}
```

然后我们得到输出:

```text
playground
Can't find ROOT
/playground/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/bin/cargo
```

所以`option_env!`永远是比较安全的宏。如果你真的想让程序在找不到环境变量时崩溃，那么`env!`会更好。



## 使用文件

现在我们在电脑上使用Rust，我们可以开始处理文件了。你会注意到，现在我们会开始在代码中越来越多的看到`Result`。这是因为一旦你开始处理文件和类似的事情，很多事情都会出错。一个文件可能不在那里，或者计算机无法读取它。

你可能还记得，如果你想使用`?`运算符，调用它的函数必须返回一个`Result`。如果你记不住错误类型，你可以什么都不给它，让编译器告诉你。让我们用一个试图用`.parse()`创建一个数字的函数来试试。

```rust
// ⚠️
fn give_number(input: &str) -> Result<i32, ()> {
    input.parse::<i32>()
}

fn main() {
    println!("{:?}", give_number("88"));
    println!("{:?}", give_number("5"));
}
```

编译器告诉我们到底该怎么做。

```text
error[E0308]: mismatched types
 --> src\main.rs:4:5
  |
3 | fn give_number(input: &str) -> Result<i32, ()> {
  |                                --------------- expected `std::result::Result<i32, ()>` because of return type
4 |     input.parse::<i32>()
  |     ^^^^^^^^^^^^^^^^^^^^ expected `()`, found struct `std::num::ParseIntError`
  |
  = note: expected enum `std::result::Result<_, ()>`
             found enum `std::result::Result<_, std::num::ParseIntError>`
```

很好! 所以我们只要把返回值改成编译器说的就可以了:

```rust
use std::num::ParseIntError;

fn give_number(input: &str) -> Result<i32, ParseIntError> {
    input.parse::<i32>()
}

fn main() {
    println!("{:?}", give_number("88"));
    println!("{:?}", give_number("5"));
}
```

现在程序可以运行了!

```text
Ok(88)
Ok(5)
```

所以现在我们想用`?`，如果能用就直接给我们数值，如果不能用就给错误。但是如何在`fn main()`中做到这一点呢？如果我们尝试在main中使用`?`，那就不行了。

```rust
// ⚠️
use std::num::ParseIntError;

fn give_number(input: &str) -> Result<i32, ParseIntError> {
    input.parse::<i32>()
}

fn main() {
    println!("{:?}", give_number("88")?);
    println!("{:?}", give_number("5")?);
}
```

它说:

```text
error[E0277]: the `?` operator can only be used in a function that returns `Result` or `Option` (or another type that implements `std::ops::Try`)
  --> src\main.rs:8:22
   |
7  | / fn main() {
8  | |     println!("{:?}", give_number("88")?);
   | |                      ^^^^^^^^^^^^^^^^^^ cannot use the `?` operator in a function that returns `()`
9  | |     println!("{:?}", give_number("5")?);
10 | | }
   | |_- this function should return `Result` or `Option` to accept `?`
```

但实际上`main()`可以返回一个`Result`，就像其他函数一样。如果我们的函数能工作，我们不想返回任何东西(main()并没有给其他任何东西)。而如果它不工作，我们将错误返回。所以我们可以这样写:

```rust
use std::num::ParseIntError;

fn give_number(input: &str) -> Result<i32, ParseIntError> {
    input.parse::<i32>()
}

fn main() -> Result<(), ParseIntError> {
    println!("{:?}", give_number("88")?);
    println!("{:?}", give_number("5")?);
    Ok(())
}
```

不要忘了最后的`Ok(())`:这在Rust中是很常见的，它的意思是`Ok`，里面是`()`，也就是我们的返回值。现在它打印出来了:

```text
88
5
```


只用`.parse()`的时候不是很有用，但是用文件就很有用。这是因为`?`也为我们改变了错误类型。下面是用简单英语写的[?运算符页面](https://doc.rust-lang.org/std/macro.try.html):

```text
If you get an `Err`, it will get the inner error. Then `?` does a conversion using `From`. With that it can change specialized errors to more general ones. The error it gets is then returned.
```

另外，Rust在使用`File`s和类似的东西时，有一个方便的`Result`类型。它叫做`std::io::Result`，当你在使用`?`对文件进行打开和操作时，通常在`main()`中看到的就是这个。这其实是一个类型别名。它的样子是这样的:

```text
type Result<T> = Result<T, Error>;
```

所以这是一个`Result<T, Error>`，但我们只需要写出`Result<T>`部分。

现在让我们第一次尝试使用文件。`std::fs`是处理文件的方法所在，有了`std::io::Write`，你就可以写。有了它，我们就可以用`.write_all()`来写进文件。

```rust
use std::fs;
use std::io::Write;

fn main() -> std::io::Result<()> {
    let mut file = fs::File::create("myfilename.txt")?; // Create a file with this name.
                                                        // CAREFUL! If you have a file with this name already,
                                                        // it will delete everything in it.
    file.write_all(b"Let's put this in the file")?;     // Don't forget the b in front of ". That's because files take bytes.
    Ok(())
}
```

然后如果你打开新文件`myfilename.txt`，会看到内容`Let's put this in the file`。

不过我们不需要写两行，因为我们有`?`操作符。如果有效，它就会传递我们想要的结果，有点像在迭代器上很多方法一样。这时候`?`就变得非常方便了。

```rust
use std::fs;
use std::io::Write;

fn main() -> std::io::Result<()> {
    fs::File::create("myfilename.txt")?.write_all(b"Let's put this in the file")?;
    Ok(())
}
```

所以这是说 "请尝试创建一个文件，然后检查是否成功。如果成功了，那就使用`.write_all()`，然后检查是否成功。"

而事实上，也有一个函数可以同时做这两件事。它叫做`std::fs::write`。在它里面，你给它你想要的文件名，以及你想放在里面的内容。再次强调，要小心! 如果该文件已经存在，它将删除其中的所有内容。另外，它允许你写一个`&str`，前面不写`b`，因为这个:

```rust
pub fn write<P: AsRef<Path>, C: AsRef<[u8]>>(path: P, contents: C) -> Result<()>
```

`AsRef<[u8]>`就是为什么你可以给它任何一个。

很简单的:

```rust
use std::fs;

fn main() -> std::io::Result<()> {
    fs::write("calvin_with_dad.txt", 
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;

    Ok(())
}
```

所以这就是我们要用的文件。这是一个名叫Calvin的漫画人物和他爸爸的对话，他爸爸对他的问题并不认真。有了这个，每次我们都可以创建一个文件来使用。



打开一个文件和创建一个文件一样简单。你只要用`open()`代替`create()`就可以了。之后(如果它找到了你的文件)，你就可以做`read_to_string()`这样的事情。要做到这一点，你可以创建一个可变的 `String`，然后把文件读到那里。它看起来像这样:

```rust
use std::fs;
use std::fs::File;
use std::io::Read; // this is to use the function .read_to_string()

fn main() -> std::io::Result<()> {
     fs::write("calvin_with_dad.txt", 
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;


    let mut calvin_file = File::open("calvin_with_dad.txt")?; // Open the file we just made
    let mut calvin_string = String::new(); // This String will hold it
    calvin_file.read_to_string(&mut calvin_string)?; // Read the file into it

    calvin_string.split_whitespace().for_each(|word| print!("{} ", word.to_uppercase())); // Do things with the String now

    Ok(())
}
```

会打印:

```rust
CALVIN: DAD, HOW COME OLD PHOTOGRAPHS ARE ALWAYS BLACK AND WHITE? DIDN'T THEY HAVE COLOR FILM BACK THEN? DAD: SURE THEY DID. IN 
FACT, THOSE PHOTOGRAPHS *ARE* IN COLOR. IT'S JUST THE *WORLD* WAS BLACK AND WHITE THEN. CALVIN: REALLY? DAD: YEP. THE WORLD DIDN'T TURN COLOR UNTIL SOMETIMES IN THE 1930S...
```

好吧，如果我们想创建一个文件，但如果已经有另一个同名的文件就不做了怎么办？也许你不想为了创建一个新的文件而删除已经存在的其他文件。要做到这一点，有一个结构叫`OpenOptions`。其实，我们一直在用`OpenOptions`，却不知道。看看`File::open`的源码吧。

```rust
pub fn open<P: AsRef<Path>>(path: P) -> io::Result<File> {
        OpenOptions::new().read(true).open(path.as_ref())
    }
```

有意思，这好像是我们学过的建造者模式。`File::create`也是如此。

```rust
pub fn create<P: AsRef<Path>>(path: P) -> io::Result<File> {
        OpenOptions::new().write(true).create(true).truncate(true).open(path.as_ref())
    }
```

如果你去[OpenOptions的页面](https://doc.rust-lang.org/std/fs/struct.OpenOptions.html)，你可以看到所有可以选择的方法。大多数采取`bool`。


- `append()`: 意思是 "添加到已经存在的内容中，而不是删除"。
- `create()`: 这让 `OpenOptions` 创建一个文件。
- `create_new()`: 意思是只有在文件不存在的情况下才会创建文件。
- `read()`: 如果你想让它读取文件，就把这个设置为 `true`。
- `truncate()`: 如果你想在打开文件时把文件内容剪为0(删除内容)，就把这个设置为true。
- `write()`: 这可以让它写入一个文件。

然后在最后你用`.open()`加上文件名，就会得到一个`Result`。我们来看一个例子。

```rust
// ⚠️
use std::fs;
use std::fs::OpenOptions;

fn main() -> std::io::Result<()> {
     fs::write("calvin_with_dad.txt", 
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;

    let calvin_file = OpenOptions::new().write(true).create_new(true).open("calvin_with_dad.txt")?;

    Ok(())
}
```

首先我们用`new`做了一个`OpenOptions`(总是以`new`开头)。然后我们给它的能力是`write`。之后我们把`create_new()`设置为`true`，然后试着打开我们做的文件。打不开，这是我们想要的。

```text
Error: Os { code: 80, kind: AlreadyExists, message: "The file exists." }
```

让我们尝试使用`.append()`，这样我们就可以向一个文件写入。为了写入文件，我们可以使用 `.write_all()`，这是一个尝试写入你给它的一切内容的方法。

另外，我们将使用 `write!` 宏来做同样的事情。你会记得这个宏，我们在为结构体做`impl Display`的时候用到过。这次我们是在文件上使用它，而不是在缓冲区上。

```rust
use std::fs;
use std::fs::OpenOptions;
use std::io::Write;

fn main() -> std::io::Result<()> {
    fs::write("calvin_with_dad.txt", 
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;

    let mut calvin_file = OpenOptions::new()
        .append(true) // Now we can write without deleting it
        .read(true)
        .open("calvin_with_dad.txt")?;
    calvin_file.write_all(b"And it was a pretty grainy color for a while too.\n")?;
    write!(&mut calvin_file, "That's really weird.\n")?;
    write!(&mut calvin_file, "Well, truth is stranger than fiction.")?;

    println!("{}", fs::read_to_string("calvin_with_dad.txt")?);

    Ok(())
}
```

这个打印:

```text
Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...And it was a pretty grainy color for a while too.
That's really weird.
Well, truth is stranger than fiction.
```

## cargo文档

你可能已经注意到，Rust文档看起来总是几乎一样。在左边你可以看到`struct`和`trait`，代码例子在右边等等。这是因为你只要输入`cargo doc`就可以自动创建文档。

即使是创建一个什么都不做的项目，也可以帮助你了解Rust中的特性。例如，这里有两个几乎什么都不做的结构体，以及一个也什么都不做的`fn main()`。

```rust
struct DoesNothing {}
struct PrintThing {}

impl PrintThing {
    fn prints_something() {
        println!("I am printing something");
    }
}

fn main() {}
```


但如果你输入`cargo doc --open`，你可以看到比你想象中更多的信息。首先它给你显示的是这样的:

```text
Crate rust_book

Structs
DoesNothing
PrintThing

Functions
main
```

但是如果你点击其中的一个结构，会让你看到很多你没有想到的trait。

```text
Struct rust_book::DoesNothing
[+] Show declaration
Auto Trait Implementations
impl RefUnwindSafe for DoesNothing
impl Send for DoesNothing
impl Sync for DoesNothing
impl Unpin for DoesNothing
impl UnwindSafe for DoesNothing
Blanket Implementations
impl<T> Any for T
where
    T: 'static + ?Sized,
[src]
[+]
impl<T> Borrow<T> for T
where
    T: ?Sized,
[src]
[+]
impl<T> BorrowMut<T> for T
where
    T: ?Sized,
[src]
[+]
impl<T> From<T> for T
[src]
[+]
impl<T, U> Into<U> for T
where
    U: From<T>,
[src]
[+]
impl<T, U> TryFrom<U> for T
where
    U: Into<T>,
[src]
[+]
impl<T, U> TryInto<U> for T
where
    U: TryFrom<T>,
```

这是因为Rust自动为每个类型实现的所有trait。

那么如果我们添加一些文档注释，当你输入`cargo doc`的时候就可以看到。

```rust
/// This is a struct that does nothing
struct DoesNothing {}
/// This struct only has one method.
struct PrintThing {}
/// It just prints the same message.
impl PrintThing {
    fn prints_something() {
        println!("I am printing something");
    }
}

fn main() {}
```


现在会打印:

```text
Crate rust_book
Structs
DoesNothing This is a struct that does nothing
PrintThing  This struct only has one method.
Functions
main
```

当你使用很多别人的crate时，`cargo doc`是非常好的。因为这些crate都在不同的网站上，可能需要一些时间来搜索所有的crate。但如果你使用`cargo doc`，你就会把它们都放在你硬盘的同一个地方。

## 结束了吗？

简单英语学Rust就这样结束了。但是我还在这里，如果你有什么问题可以告诉我。欢迎[在Twitter上联系我](https://twitter.com/mithridates)或者添加一个pull request、issue等。如果有些地方不容易理解，你也可以告诉我。简单英语学Rust需要非常容易理解，所以请告诉我英语太难的地方。当然，Rust本身也可能是很难理解的，但我们至少可以确保英语是容易的。

