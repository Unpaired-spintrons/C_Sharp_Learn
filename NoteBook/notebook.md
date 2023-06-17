# Lcs的C#奇妙冒险

## 编程哲学

> 我认为C#和Rust有些相似，都是以类内部的操作作为一个函数调用，采用如图C++一样的命名空间进行操作（？），目前看来还挺好玩。
>
> 2023.6.9 10:25

## 函数笔记

### 官方库

#### Console命名空间

##### Console.WriteLine()

在命令行上写入一段话

###### Console.WriteLine("文字")

将文字显示在命令行上


## 数据类型

C#是使用一种和C++一样的独特编程方法，他们的值可以被任意定义，这主要是因为他们包含了类，其实在编写的时候我们只是在进行类成员的编写。所以我们可以使用不同类型的成员以此来进行不同类型的操作例子：(使用C++)

```C++
Class Hello
{
public:
    Hello();
    int value1;
    float value2;
    int A(int a, int b);
    ```
    ~Hello();
}  
```

在微软的文档中显示我们的C#需要成员，函数，初始化和节数函数，这很C++，或者是C的 **struct** 的进化吧！

> C#的数据主要分为两个类型 **引用类型** **值类型**
>
> @是C#的保留字

### 值类型

> 这个类型的值每一个都有自己独立的副本。简单来说他们就像一个一个的个体我改变一个个体的值对于另一个个体的值没有影响。


### 引用类型

> 这个类型是类似于一体同心，我改了这个值，大家都会变，会影响，还和虫族不一样，他是每个都平等，不是像虫族还有主副之分




## 示例项目

### VS使用

#### 新建项目

##### 命令行项目

![img](img\新建C_Sharp命令行项目.png)

### Hello World!

```C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp_Hello_World_
{
	class Program
	{
		static void Main(string[] args)
		{
			Console.WriteLine("你好，世界");
		}
	}
}

```

#### 有趣之处

这个和早期的C一样，好像VS并没有对他进行像尾部加getchar这样的优化，所以调试窗口会一闪而过，但是我们可以在VS项目中的bin/debug目录下找到exe并且采用命令行运行他们。

![img](img\命令行程序在命令行中运行.png)
