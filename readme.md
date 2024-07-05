## 写在前面
译者在学习python时，发现了此教程，觉得写的非常细致，很适合python入门。所以决定尝试着翻译此教程。原作者是 [Asabeneh](https://github.com/Asabeneh) ，原文[链接](https://github.com/Taki-Ta/30-Days-Of-Python)。

译者英文水平有限，翻译难免有错误，欢迎指正。

因为译者在上班外的空闲时间进行翻译工作，难免进度缓慢，如果你想加入到翻译工作中来，可以通过创建 pr ，指定要翻译的章节，我会尽快合并。

如果你觉得这个教程对你有所帮助，可以给我一个star。

# 🐍 30 Days Of Python


|# Day | 标题                                                    |
|------|:---------------------------------------------------------:|
| 01  |  [介绍](./readme.md)|
| 02  |  [变量, 内置函数](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)|
| 03  |  [运算符](./03_Day_Operators/03_operators.md)|
| 04  |  [Strings](./04_Day_Strings/04_strings.md)|
| 05  |  [Lists](./05_Day_Lists/05_lists.md)|
| 06  |  [Tuples](./06_Day_Tuples/06_tuples.md)|
| 07  |  [Sets](./07_Day_Sets/07_sets.md)|
| 08  |  [Dictionaries](./08_Day_Dictionaries/08_dictionaries.md)|
| 09  |  [Conditionals](./09_Day_Conditionals/09_conditionals.md)|
| 10  |  [Loops](./10_Day_Loops/10_loops.md)|
| 11  |  [Functions](./11_Day_Functions/11_functions.md)|
| 12  |  [Modules](./12_Day_Modules/12_modules.md)|
| 13  |  [List Comprehension](./13_Day_List_comprehension/13_list_comprehension.md)|
| 14  |  [Higher Order Functions](./14_Day_Higher_order_functions/14_higher_order_functions.md)|
| 15  |  [Python Type Errors](./15_Day_Python_type_errors/15_python_type_errors.md)|
| 16 |  [Python Date time](./16_Day_Python_date_time/16_python_datetime.md) |
| 17 |  [Exception Handling](./17_Day_Exception_handling/17_exception_handling.md)|
| 18 |  [Regular Expressions](./18_Day_Regular_expressions/18_regular_expressions.md)|
| 19 |  [File Handling](./19_Day_File_handling/19_file_handling.md)|
| 20 |  [Python Package Manager](./20_Day_Python_package_manager/20_python_package_manager.md)|
| 21 |  [Classes and Objects](./21_Day_Classes_and_objects/21_classes_and_objects.md)|
| 22 |  [Web Scraping](./22_Day_Web_scraping/22_web_scraping.md)|
| 23 |  [Virtual Environment](./23_Day_Virtual_environment/23_virtual_environment.md)|
| 24 |  [Statistics](./24_Day_Statistics/24_statistics.md)|
| 25 |  [Pandas](./25_Day_Pandas/25_pandas.md)|
| 26 |  [Python web](./26_Day_Python_web/26_python_web.md)|
| 27 |  [Python with MongoDB](./27_Day_Python_with_mongodb/27_python_with_mongodb.md)|
| 28 |  [API](./28_Day_API/28_API.md)|
| 29 |  [Building API](./29_Day_Building_API/29_building_API.md)|
| 30 |  [Conclusions](./30_Day_Conclusions/30_conclusions.md)|

🧡🧡🧡 下面是原作者的paypal账户 🧡🧡🧡

<div>
<small>支持 <strong>作者</strong> 创造更多教程</small> <br />  
<a href = "https://www.paypal.me/asabeneh"><img src='./images/paypal_lg.png' alt='Paypal Logo' style="width:10%"/></a>
</div>

<div align="center">
  <h1> 30 Days Of Python：第一天 - 介绍</h1>
  <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/asabeneh/">
  <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
  </a>
  <a class="header-badge" target="_blank" href="https://twitter.com/Asabeneh">
  <img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/asabeneh?style=social">
  </a>

  <sub>Author:
  <a href="https://www.linkedin.com/in/asabeneh/" target="_blank">Asabeneh Yetayeh</a><br>
  <small> Second Edition: July, 2021</small>
  </sub>
</div>

[第二天 >>](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)

![30DaysOfPython](./images/30DaysOfPython_banner3@2x.png)

_阅读大约需要：21m_

- [🐍 30 Days Of Python](#-30-days-of-python)
- [📘 第一天](#-第一天)
  - [欢迎](#欢迎)
  - [介绍](#介绍)
  - [为什么选择Python?](#为什么选择-python)
  - [环境配置](#环境配置)
    - [安装 Python](#安装-python)
    - [Python Shell](#python-shell)
    - [安装 Visual Studio Code](#安装-visual-studio-code)
      - [如何使用 visual studio code](#如何使用-visual-studio-code)
  - [Python 基础](#python-基础)
    - [Python 语法](#python-syntax)
    - [Python 缩进](#python-indentation)
    - [注释](#comments)
    - [数据类型](#data-types)
      - [Number](#number)
      - [String](#string)
      - [Booleans](#booleans)
      - [List](#list)
      - [Dictionary](#dictionary)
      - [Tuple](#tuple)
      - [Set](#set)
    - [检查数据类型](#检查数据类型)
    - [Python 文件](#python-文件)
  - [💻 练习 - 第一天](#-练习---第一天)
    - [练习： 1级](#练习-1级)
    - [练习： 2级](#练习-2级)
    - [练习： 3级](#练习-3级)

# 📘 第一天

## 欢迎

**恭喜** 您决定参加 _30 days of Python_ 编程挑战赛。 在这次挑战赛中，您将学习成为 Python 程序员所需的一切以及编程的整个概念。挑战赛结束时，您将获得 _30DaysOfPython_ 编程挑战赛证书。

如果你想积极参与挑战，你可以加入 [30DaysOfPython challenge](https://t.me/ThirtyDaysOfPython) telegram 群组。

## 介绍

Python 是一中通用的高级编程语言。它是一种开源、解释型、面向对象的编程语言。Python 是由荷兰程序员 Guido van Rossum 创建的。Python 编程语言的名称源自英国小品喜剧系列《Monty Python's Flying Circus》。 第一个版本于 1991 年 2 月 20 日发布。这个为期 30 天的 Python 挑战将帮助您逐步学习最新版本的 Python ，即 Python 3。主题分为 30 天，每天包含几个主题，并附有易于理解的解释、真实示例、许多动手练习和项目。

本次挑战赛针对想要学习 Python 编程语言的初学者和专业人士。完成挑战可能需要 30 到 100 天，积极参与 telegram 群组的人完成挑战的概率很高。

这项挑战易于阅读，以会话英语编写，引人入胜、激励人心，同时要求很高。您需要留出大量时间来完成。如果你想看视频学习，你可以在 <a href="https://www.youtube.com/channel/UC7PNRuno1rzYPb1xLa4yktw"> Washera</a> YouTube 频道获取视频教程。也可以从 [Python for Absolute Beginners video](https://youtu.be/OCCWZheOesI) 开始学习。 订阅频道，在 YouTube 视频上发表评论和提问，并积极主动，作者最终会注意到你。

作者希望听到你们的看法，分享作者以表达你对此教程的看法。 你可以在这个[链接](https://testimonial-vdzd.onrender.com/)留言。

## 为什么选择 Python?

它是一种非常接近人类语言的编程语言，因此易于学习使用。
Python 被大量行业、公司使用 (包括 Google 在内)。它已被用于开发 Web 应用程序、桌面应用程序、系统管理和机器学习库。Python 是数据科学和机器学习社区中备受推崇的语言。希望这足以说服您开始学习 Python。 Python is eating the world and you are killing it before it eats you（太中二了，不知道该怎么翻译 :) ）.

## 环境配置

### 安装 Python

为了运行 Python 脚本，你需要安装 python 。在这里 [下载](https://www.python.org/) python.
如果你使用的是 Windows 系统，点击红框中的按钮。

[![installing on Windows](./images/installing_on_windows.png)](https://www.python.org/)

如果你使用的是 macOS 系统， 点击下面红框中的按钮。

[![installing on Windows](./images/installing_on_macOS.png)](https://www.python.org/)

为了确认 Python 是否安装成功，你可以在终端中输入以下命令。

```shell
python --version
```

![Python Version](./images/python_versio.png)

如上图所示，我目前使用的是 _Python 3.7.5_ 版本。你的 Python 版本可能与我的不同，但应该是 3.6 或更高版本。如果你能看到 Python 版本，那么恭喜你。Python 已经安装在你的计算机上。继续下一节。


### Python Shell

Python 是一种解释型脚本语言，因此不需要编译。这意味着它逐行执行代码。Python 自带一个 _Python Shell (Python 交互式 Shell)_。它用于执行单个 Python 命令并获取结果。

Python Shell 等待用户输入 Python 代码。当你输入代码时，它会解释代码并在下一行显示结果。

打开你的终端或命令提示符(cmd)，输入：

```shell
python
```

![Python Scripting Shell](./images/opening_python_shell.png)

打开 Python 交互式 Shell ，控制台会等待你输入 Python 代码（Python 脚本）。你可以在这个符号 >>> 后输入你的 Python 代码（Python 脚本），然后点击 Enter。

让我们在 Python Script shell 上写我们的第一个脚本。

![Python script on Python shell](./images/adding_on_python_shell.png)

恭喜你，你在 Python 交互式 Shell 上写了你的第一个 Python 脚本。如何关闭 Python 交互式 Shell ? 为了关闭 Shell，在这个符号 >>> 旁边输入 **exit()** 命令，然后按 Enter。

![Exit from python shell](./images/exit_from_shell.png)

现在，你知道如何打开 Python 交互式 Shell 以及如何退出。

Python 会在你写的脚本中给你结果，如果你写的是 Python 能理解的脚本，否则会返回错误。让我们故意犯一个错误，看看 Python 会返回什么。

![Invalid Syntax Error](./images/invalid_syntax_error.png)

正如你从返回的错误中看到的，Python 是如此聪明，它知道我们犯的错误，这个错误是 _Syntax Error: invalid syntax_. 在 Python 中使用 x 作为乘法是一个语法错误，因为 (x) 不是 Python 中的有效语法。我们应该使用星号 (*) 代替 x 来表示乘法。返回的错误清楚地显示了需要修复的地方。

从程序中识别并修改的过程称为 _调试_。让我们通过在 **x** 的位置放 * 来调试它。


![Fixing Syntax Error](./images/fixing_syntax_error.png)

我们的错误已经修复，代码运行并得到了我们期望的结果。作为程序员，你每天都会遇到这种错误。了解如何调试是很重要的。要成为一个优秀的调试者，你应该了解你遇到的错误类型。下面的错误你可能已经处理过了 _SyntaxError_， _IndexError_， _NameError_， _ModuleNotFoundError_， _KeyError_， _ImportError_， _AttributeError_， _TypeError_， _ValueError_， _ZeroDivisionError_ 等。 我们将在后面的章节中详细了解不同的 Python **_错误类型_**。

让我们继续练习如何使用 Python 交互式 Shell。打开你的终端或命令提示符(cmd)，输入：


![Python Scripting Shell](./images/opening_python_shell.png)

Python 交互式 Shell 已经打开。让我们在 Shell 上做一些基本的数学运算（加法、减法、乘法、除法、取余、指数）。

在我们写任何 Python 代码之前，让我们先做一些数学运算：

- 2 + 3 = 5
- 3 - 2 = 1
- 3 \* 2 = 6
- 3 / 2 = 1.5
- 3 ** 2 = 3 * 3

在 Python 中我们有以下额外的操作：

- 3 % 2 = 1 => 获取余数
- 3 // 2 = 1 => Floor除法，返回商的整数部分

让我们把上面的数学表达式转换成 Python 代码。Python Shell 已经打开，让我们在 Shell 上写代码。

在 python 中，_注释_ 是代码的一部分，不会被 python 执行。所以我们可以在我们的代码中留下一些文本，使我们的代码更易读。Python 不会运行注释部分。Python 中的注释以井号(#)符号开头。

在 python 中，我们这样编写注释：

```shell
 # 注释以 (#) 开始
 # 这是一个 python 注释，因为它以 (#) 符号开始
```

![Maths on python shell](./images/maths_on_python_shell.png)


在进入下一节之前，让我们在 Python 交互式 shell 上多练习一下。通过在 shell 上写入 _exit()_ 关闭打开的 shell，然后再次打开它，让我们练习如何在 Python shell 上编写文本。

![Writing String on python shell](./images/writing_string_on_shell.png)

### 安装 Visual Studio Code

Python 交互式 shell 适合尝试和测试小的脚本代码，但不适合大型项目。在真实的工作环境中，开发人员使用不同的代码编辑器来编写代码。在这 30 天的 Python 编程挑战中，我们将使用 Visual Studio Code。Visual Studio Code 是一个非常流行的开源文本编辑器。我是 Visual Studio Code 的粉丝，我推荐你 [下载](https://code.visualstudio.com/) Visual Studio Code，但如果你喜欢其他编辑器，使用你喜欢的就可以。

[![Visual Studio Code](./images/vscode.png)](https://code.visualstudio.com/)

如果你安装了 Visual Studio Code，让我们看看如何使用它。
如果你更喜欢视频，你可以观看这个 Visual Studio Code for Python [视频教程](https://www.youtube.com/watch?v=bn7Cx4z-vSo)


#### 如何使用 visual studio code

双击打开 visual studio code 图标，你会看到这样的界面。试着使用图标进行操作。

![Visual studio Code](./images/vscode_ui.png)

在桌面上创建一个名为 30DaysOfPython 的文件夹，然后在 visual studio code 中打开。

![Opening Project on Visual studio](./images/how_to_open_project_on_vscode.png)

![Opening a project](./images/opening_project.png)

打开后，你会看到 30DaysOfPython 项目的目录。如下图所示，我已经创建了第一个文件 helloworld.py。你也可以这样做。

![Creating a python file](./images/helloworld.png)

经过一天的编码后，你想关闭代码编辑器，对吧？可以这样关闭打开的项目。

![Closing project](./images/closing_opened_project.png)

恭喜你，你已经完成了开发环境的设置。让我们开始写代码吧。

## Python 基础

### Python 语法

Python 脚本可以在 Python 交互式 shell 中编写，也可以在代码编辑器中编写。Python 文件的扩展名是 .py。

### Python 缩进

_缩进_ 就是文本中的空格。在许多编程语言中，_缩进_ 常用于增加代码的可读性，但在 Python 中，缩进用于创建代码块。在其他编程语言中使用 {} 来创建代码块。在编写 Python 代码时，最常见的 bug 之一就是错误缩进。

![Indentation Error](./images/indentation.png)

### 注释

注释对于使代码更易读和在代码中留下备注非常重要。Python 不会运行注释部分。在 Python 中，任何以 # 开头的文本都是注释。

**示例： 单行注释**

```shell
    # 第一行注释
    # 第二行注释
    # Python 正在吞噬这个世界
```

**示例： 多行注释**

如果没有赋值给变量，三个引号可以用于多行注释。


```shell
"""这是一个多行注释
多行注释有多行
Python 正在吞噬这个世界
"""
```

### 数据类型

在 Python 中有几种数据类型。让我们从最常见的数据类型开始。其他数据类型将在之后的章节中详细介绍。现在，我们来看一下不同的数据类型，并熟悉它们。你现在不必完全掌握。

#### Number

- Integer： 整型数字(负数， 0 以及 正数)
    示例：
    ... -3, -2, -1, 0, 1, 2, 3 ...
- Float： 浮点数
    示例
    ... -3.5, -2.25, -1.0, 0.0, 1.1, 2.2, 3.5 ...
- Complex： 复数
    示例
    1 + j, 2 + 4j

#### String

 字符串是一个或多个字符的集合，用单引号或双引号括起来。如果字符串有多行，需要使用三引号。
A collection of one or more characters under a single or double quote. If a string is more than one sentence then we use a triple quote.

**示例：**

```py
'Asabeneh'
'Finland'
'Python'
'I love teaching'
'I hope you are enjoying the first day of 30DaysOfPython Challenge'
```

#### Booleans

布尔数据类型是 True 或 False 值。T 和 F 应该始终大写。

**示例：**

```python
    True  #  灯开着吗? 如果开着，值应该是 True
    False #  灯开着吗? 如果开着，值应该是 False
```

#### List

Python 列表是一个有序的集合，允许存储不同数据类型的项。列表类似于 JavaScript 中的数组。

**示例：**

```py
[0, 1, 2, 3, 4, 5]  # 所有元素都是相同的类型 - 一个数组列表
['Banana', 'Orange', 'Mango', 'Avocado'] # 所有元素都是相同的类型 - 一个字符串列表
['Finland','Estonia', 'Sweden','Norway'] # 所有元素都是相同的类型 - 一个字符串列表
['Banana', 10, False, 9.81] # 列表中有不同数据类型的元素 - 字符串、整数、布尔值和浮点数
```

#### Dictionary

Python 字典对象是一个无序的数据集合，以键值对的形式存储数据。

**示例：**

```py
{
'first_name':'Asabeneh',
'last_name':'Yetayeh',
'country':'Finland', 
'age':250, 
'is_married':True,
'skills':['JS', 'React', 'Node', 'Python']
}
```

#### Tuple

元组是一个有序的不同数据类型的集合，类似于列表，但元组一旦创建就不能修改。它们是不可变的。

**示例：**

```py
('Asabeneh', 'Pawel', 'Brook', 'Abraham', 'Lidiya') # 姓名
```

```py
('Earth', 'Jupiter', 'Neptune', 'Mars', 'Venus', 'Saturn', 'Uranus', 'Mercury') # 星球
```


#### Set

集合是一组类似于列表和元组的数据类型。与列表和元组不同，集合不是有序的数据集合。与数学中的集合类似，集合中只存储唯一的项。

在之后的章节中，我们会详细了解 Python 中的每个数据类型。


**示例：**

```py
{2, 4, 3, 5}
{3.14, 9.81, 2.7} # order is not important in set
```

### 检查数据类型

为了检查某些数据/变量的数据类型，我们使用 **type** 函数。在下面的终端中，你将看到不同的 python 数据类型：

![Checking Data types](./images/checking_data_types.png)

### Python 文件

首先打开你的项目文件夹，30DaysOfPython。如果你没有这个文件夹，需要创建一个。在这个文件夹中创建一个名为 helloworld.py 的文件。现在，让我们在 Visual Studio Code 上做我们在 Python 交互式 shell 上做的事情。

在 Python 交互式 shell 上，不使用 **print** 也可以打印，但在 Visual Studio Code 上，为了看到我们的结果，我们应该使用内置函数 _print()_。_print()_ 内置函数接受一个或多个参数，如下所示 _print('arument1','argument2','argument3')_。下面是使用示例。


**示例：**

文件名为 helloworld.py

```py
# Day 1 - 30DaysOfPython Challenge

print(2 + 3)             # 加(+)
print(3 - 1)             # 减(-)
print(2 * 3)             # 乘(*)
print(3 / 2)             # 除(/)
print(3 ** 2)            # 指数运算(**)
print(3 % 2)             # 求模(%)
print(3 // 2)            # Floor除法(//)

# 检查数据类型
print(type(10))          # 整形
print(type(3.14))        # 浮点型
print(type(1 + 3j))      # 复数
print(type('Asabeneh'))  # 字符串
print(type([1, 2, 3]))   # 列表
print(type({'name':'Asabeneh'})) # 字典类型
print(type({9.8, 3.14, 2.7}))    # 集合
print(type((9.8, 3.14, 2.7)))    # 元组
```

要运行 python 文件，请查看下面的图片。你可以通过在 Visual Studio Code 上运行绿色按钮或在终端中输入 _python helloworld.py_ 来运行 python 文件。

![Running python script](./images/running_python_script.png)

🌕 你太棒了。在成功的路上，你刚刚完成了第一天的挑战。现在做些锻炼大脑和肌肉的练习吧。


## 💻 练习 - 第一天

### 练习： 1级

1. 检查你正在使用的 Python 版本。
2. 打开 python 交互式 shell ，执行以下操作。重复3、4遍。
   - 加法(+)
   - 减法(-)
   - 乘法(\*)
   - 模运算(%)
   - 除法(/)
   - 指数运算(\*\*)
   - Floor 除法(//)
3. 在 python 交互式 shell 中输入以下字符串：
   - 你的名字
   - 你的姓氏
   - 你的国籍
   - 我正在享受 30 days of python 课程
4. 检查下列数据的数据类型：
   - 10
   - 9.8
   - 3.14
   - 4 - 4j
   - ['Asabeneh', 'Python', 'Finland']
   - 你的名字
   - 你的姓氏
   - 你的国籍

### 练习： 2级

1. 在 30DaysOfPython 文件夹内创建一个名为 day_1 的文件夹。在 day_1 文件夹内创建一个名为 helloworld.py 的 python 文件，并重复问题 1、2、3、4。记得在 python 文件中使用 _print()_。导航到你保存文件的目录，并运行它。

### 练习： 3级


1. 为不同的 Python 数据类型编写一个示例，例如 Number(Integer， Float， Complex)， String， Boolean， List， Tuple， Set and Dictionary.
2. 算出 (2, 3) 和 (10, 8)间的 [欧几里得距离](https://en.wikipedia.org/wiki/Euclidean_distance#:~:text=In%20mathematics%2C%20the%20Euclidean%20distance,being%20called%20the%20Pythagorean%20distance.) 

🎉 恭喜 ! 🎉

[第二天 >>](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)
