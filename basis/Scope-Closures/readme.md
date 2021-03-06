# closure 闭包

## 作用域
1. 全局作用域
2. 函数作用域
3. eval、with
4. try/catch
5. let、const

## 词法作用域
1. 词法作用域是作用域的一种工作模型。
2. 词法作用域就是作用域是由书写代码时函数声明的位置来决定的。
3. 编译阶段就能够知道全部标识符在哪里以及是如何声明的，所以词法作用域是静态的作用域，也就是词法作用域能够预测在执行代码的过程中如何查找标识符。

## 什么是闭包
### 《JavaScript高级程序设计》这样描述
> 闭包是指有权访问另一个函数作用域中的变量的函数；
### 《JavaScript权威指南》这样描述：
> 从技术的角度讲，所有的JavaScript函数都是闭包：它们都是对象，它们都关联到作用域链。
### 《你不知道的JavaScript》这样描述：
> 当函数可以记住并访问所在的词法作用域时，就产生了闭包，即使函数是在当前词法作用域之外执行。

我最认同的是《你不知道的JavaScript》中的描述，虽然前面的两种说法都没有错，但闭包应该是基于词法作用域书写代码时产生的自然结果，是一种现象！你也不用为了利用闭包而特意的创建，因为闭包的在你的代码中随处可见，只是你还不知道当时你写的那一段代码其实就产生了闭包。

### 闭包的应用
1、 设置私有的属性, 用于定义模块，我们将操作函数暴露给外部，而细节隐藏在模块内部
2、 单例应用
## 参考资料
1. [作用域与词法作用域](https://juejin.im/post/5afb0ae56fb9a07aa2138425)
2. [包详解一](https://juejin.im/post/5b081f8d6fb9a07a9b3664b6)