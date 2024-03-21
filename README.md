# Python-for-web

### setting the python pathway

**Due to I used the Annocaonda to intall python in the Windows**

So I would like to activate conda before create a env.

首先，需要在搜索里面找到**Anaconda Promoter**的命令框，然后再里面运行命令

```
#这是创建的
conda create -n 环境的名字 python=3.8
#后面的python版本号可以改
```

## 基础语法

**Python 是一种区分大小写的编程语言。因此，Manpower和manpower在 Python 中是两个不同的标识符**

- Python 类名称以大写字母开头。所有其他标识符都以小写字母开头。

- 以单个前导下划线开头的标识符表示该标识符是私有标识符。

- 以两个前导下划线开头的标识符表示强私有标识符。

- 如果标识符也以两个尾部下划线结尾，则该标识符是语言定义的特殊名称。


**Python 行和缩进**

Python 编程不提供大括号来指示类和函数定义或流程控制的代码块。代码块由严格执行的行缩进表示。

缩进中的空格数是可变的，但块中的所有语句必须缩进相同的数量。

意思就是，缩进相同的才是一个模块，比它缩进少的命令行就是它的上支.

```PYTHON
import sys

try:
   # open file stream
   file = open(file_name, "w")
except IOError:
   print "There was an error writing to", file_name
   sys.exit()
print "Enter '", file_finish,
print "' When finished"
while file_text != file_finish:
   file_text = raw_input("Enter text: ")
   if file_text == file_finish:
      # close the file
      file.close
      break
   file.write(file_text)
   file.write("\n")
file.close()
file_name = raw_input("Enter filename: ")
if len(file_name) == 0:
   print "Next time please enter something"
   sys.exit()
try:
   file = open(file_name, "r")
except IOError:
   print "There was an error reading file"
   sys.exit()
file_text = file.read()
file.close()
print file_text

```

**关于python的换行**

- 在没有（），[],{},的时候，需要在结尾加上“\”作为换行符。
- 而在有以上符号时候，不用使用换行符号.

```
total = item_one + \
        item_two + \
        item_three
```

```
days = ['Monday', 'Tuesday', 'Wednesday',
        'Thursday', 'Friday']
```

**关于如何在python中写注释**

- 首先当然是“#” 这是常见的注释标识
- 其次就是python特色的多行注释了：'''

```
# This is a comment.
# This is a comment, too.
# This is a comment, too.
# I said that already.

'''
This is a multiline
comment.
'''
```

