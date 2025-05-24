# .MUSIC Pythoncode - Beta 1.0.0

## 简介

.MUSIC Pythoncode 是一个基于 Python 开发的自定义解释器，专注于提供广泛的功能和出色的易用性。它支持执行类 Python 代码和特定的 `.pymu` 脚本文件，适用于教育、简单脚本编写、图形绘制等多种场景。

## 功能特点

- **丰富的内置函数**：包含基础类型操作、数学计算、随机数生成等常用功能
- **文件操作支持**：可以读取和执行 `.pymu` 脚本文件
- **图形绘制能力**：集成 turtle 模块，支持基本的图形绘制
- **跨平台支持**：路径处理等功能支持 Windows 和 Linux 等主流操作系统
- **交互式模式**：提供友好的交互式命令行界面


## 快速开始

### 环境要求

- Python 3.6 或更高版本
- 以下 Python 模块（通常随 Python 安装）：
  - math
  - random
  - os
  - json
  - requests
  - sys
  - datetime
- 图形绘制相关模块：
  - turtle
  - tkinter（通常随 Python 安装）

### 安装方法

1. 直接下载 `.MUSIC Pythoncode-Beta 1.py` 文件
2. 确保已安装所需的 Python 模块
3. 无需额外安装，直接运行脚本即可

### 运行方式

#### 1. 交互式模式

```bash
python .MUSIC\ Pythoncode-Beta\ 1.py
```

进入交互式模式后，可以直接输入代码并执行：

```
>>> output('Hello, .MUSIC!')
Hello, .MUSIC!
>>> a = rtext('What\'s your name?')
What's your name? Alice
>>> output(f'Hello, {a}!')
Hello, Alice!
```

输入 `exit()` 退出交互式模式。

#### 2. 执行脚本文件

```bash
python .MUSIC\ Pythoncode-Beta\ 1.py 你的脚本.pymu
```

## 内置函数和常量

### 基础类型和操作

| 函数/常量 | 描述 |
|----------|------|
| `output` | 输出内容到控制台，相当于 Python 的 `print` |
| `rtext` | 从控制台读取用户输入，相当于 Python 的 `input` |
| `ctype` | 获取对象类型，相当于 Python 的 `type` |
| `toint` | 将对象转换为整数，相当于 Python 的 `int` |
| `tostr` | 将对象转换为字符串，相当于 Python 的 `str` |
| `tofloat` | 将对象转换为浮点数，相当于 Python 的 `float` |
| `tolist` | 将对象转换为列表，相当于 Python 的 `list` |
| `totuple` | 将对象转换为元组，相当于 Python 的 `tuple` |
| `todict` | 将对象转换为字典，相当于 Python 的 `dict` |
| `toset` | 将对象转换为集合，相当于 Python 的 `set` |
| `opfe` | 打开文件，相当于 Python 的 `open` |
| `li` | 获取可迭代对象中的最小值，相当于 Python 的 `min` |
| `bi` | 获取可迭代对象中的最大值，相当于 Python 的 `max` |

### 数学函数

| 函数/常量 | 描述 |
|----------|------|
| `sqrt` | 计算平方根，相当于 `math.sqrt` |
| `sin` | 计算正弦值，相当于 `math.sin` |
| `cos` | 计算余弦值，相当于 `math.cos` |
| `tan` | 计算正切值，相当于 `math.tan` |
| `log` | 计算自然对数，相当于 `math.log` |
| `pi` | 圆周率 π，相当于 `math.pi` |

### 随机函数

| 函数 | 描述 |
|------|------|
| `trand` | 生成 0 到 1 之间的随机浮点数，相当于 `random.random` |
| `trandom` | 生成指定范围内的随机整数，相当于 `random.randint` |
| `choice` | 从序列中随机选择一个元素，相当于 `random.choice` |

### 文件和路径操作

| 函数 | 描述 |
|------|------|
| `plistdir` | 获取目录中的文件和子目录列表，相当于 `os.listdir` |
| `pathjoin` | 拼接路径，支持跨平台，相当于 `os.path.join` |
| `cp` | 检查文件或目录是否存在，相当于 `os.path.exists` |

### JSON 操作

| 函数 | 描述 |
|------|------|
| `json_dumps` | 将 Python 对象转换为 JSON 字符串，相当于 `json.dumps` |
| `json_loads` | 将 JSON 字符串转换为 Python 对象，相当于 `json.loads` |

### HTTP 请求

| 函数 | 描述 |
|------|------|
| `reurlget` | 发送 HTTP GET 请求，相当于 `requests.get` |
| `reurlpost` | 发送 HTTP POST 请求，相当于 `requests.post` |

### 时间和日期

| 函数/常量 | 描述 |
|----------|------|
| `thistime` | 获取当前日期和时间，相当于 `datetime.now` |
| `todaytime` | 获取当前日期，相当于 `datetime.today` |
| `st` | 将字符串转换为日期时间对象，相当于 `datetime.strptime` |

### 图形绘制

| 函数 | 描述 |
|------|------|
| `picmove` | 移动画笔，相当于 `turtle.move` |
| `picdraw` | 绘制线条，相当于 `turtle.forward` |
| `piccolor` | 设置画笔颜色，相当于 `turtle.color` |
| `picpenup` | 抬起画笔，移动时不绘制，相当于 `turtle.penup` |
| `picpendown` | 放下画笔，移动时绘制，相当于 `turtle.pendown` |
| `picsetpos` | 设置画笔位置，相当于 `turtle.setpos` |
| `picsetheading` | 设置画笔朝向，相当于 `turtle.setheading` |
| `picsetx` | 设置画笔的 x 坐标，相当于 `turtle.setx` |
| `picsety` | 设置画笔的 y 坐标，相当于 `turtle.sety` |
| `picturn` | 旋转画笔，相当于 `turtle.turn` |
| `piccircle` | 绘制圆形，相当于 `turtle.circle` |
| `picbegin_fill` | 开始填充图形，相当于 `turtle.begin_fill` |
| `picend_fill` | 结束填充图形，相当于 `turtle.end_fill` |

### 自定义函数

| 函数 | 描述 |
|------|------|
| `join` | 跨平台路径拼接函数 |
| `empty` | 空函数，不执行任何操作 |
| `close` | 退出解释器 |

## 图形绘制示例

```python
# 绘制一个彩色的正方形
piccolor("red")
picbegin_fill()
for i in range(4):
    picdraw(100)
    picturn(90)
picend_fill()
```

## 脚本文件示例

创建一个 `greeting.pymu` 文件，内容如下：

```python
output('Hello! Welcome to .MUSIC Pythoncode!')
name = rtext('Please enter your name: ')
output(f'Hello, {name}! Nice to meet you.')
```

执行该脚本：

```bash
python .MUSIC\ Pythoncode-Beta\ 1.py greeting.pymu
```

## 错误处理

如果在执行过程中出现错误，解释器会显示错误信息，例如：

```
Error: division by zero
```

## 版本信息

- 版本：1.0.0 Beta 1
- 版权：©Open Code 2025-now, all rights reserved.

## 贡献和反馈

如果您发现问题或有改进建议，请通过以下方式反馈：
- 邮箱：your_email@example.com
- 问题跟踪：请在项目仓库中提交 issue

## 许可证

本项目采用 MIT 许可证 - 详见 LICENSE 文件

## 致谢

感谢 Python 社区和所有开源项目的贡献者，本项目在他们的基础上开发而成。
