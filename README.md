#这个文档是从astaxie那里复制过来的，修改以后供自己观看

# 输入输出(Input/Output)
[io包](https://github.com/iteny/gopkg/tree/master/io "点击进入")
`(I/O primitives,提供基本的接口)`<br>
[io/ioutil包](https://github.com/iteny/gopkg/tree/master/io/ioutil "点击进入")`(封装一些实用的I/O函数)`<br>
[fmt包](https://github.com/iteny/gopkg/tree/master/fmt "点击进入")`(实现格式化I/O，类似C语言中的printf和scanf)`<br>
[bufio包](https://github.com/iteny/gopkg/tree/master/bufio "点击进入")`(实现带缓冲I/O)`<br>

# 文本处理
[strings包](https://github.com/iteny/gopkg/tree/master/strings "点击进入")`(字符串操作)`<br>
[bytes包](https://github.com/iteny/gopkg/tree/master/bytes "点击进入")`(byte slice 便利操作)`<br>
[strconv包](https://github.com/iteny/gopkg/tree/master/strconv "点击进入")`(字符串和基本数据类型之间转换)`<br>
[regexp包](https://github.com/iteny/gopkg/tree/master/regexp "点击进入")`(正则表达式)`<br>
[unicode包](https://github.com/iteny/gopkg/tree/master/unicode "点击进入")`(Unicode码点、UTF-8/16编码)`<br>

# 数据结构与算法
[sort包](https://github.com/iteny/gopkg/tree/master/sort "点击进入")`(包含基本的排序方法，支持切片数据排序以及用户自定义数据集合排序)`<br>
[index/suffixarray包](https://github.com/iteny/gopkg/tree/master/index/suffixarray "点击进入")`(包实现了后缀数组相关算法以支持许多常见的字符串操作)`<br>
[container包](https://github.com/iteny/gopkg/tree/master/container "点击进入")`(包提供了对heap、list和ring这3种数据结构的底层支持。任何实现了相应接口的数据结构都可以调用该结构的方法)`<br>

# 日期与时间
[time包](https://github.com/iteny/gopkg/tree/master/time "点击进入")`(包提供了时间的显示和计量用的功能。日历的计算采用的是公历)`<br>

# 基本数学函数
[math包](https://github.com/iteny/gopkg/tree/master/math "点击进入")`(包实现的就是数学公式计算)`<br>

# 文件系统
[os包](https://github.com/iteny/gopkg/tree/master/os "点击进入")`(提供了跨平台的操作系统功能实现)`<br>

# 数据库操作
[database/sql包](https://github.com/iteny/gopkg/tree/master/database/sql "点击进入")`(这是 Go 提供的操作 SQL/SQL-Like 数据库的通用接口，但 Go 标准库并没有提供具体数据库的实现，需要结合第三方的驱动来使用该接口。本书使用的是 mysql 的驱动：github.com/go-sql-driver/mysql。注：该包有一个子包：driver，它定义了一些接口供数据库驱动实现，一般业务代码中使用 database/sql 包即可，尽量避免使用 driver 这个子包。)`<br>

# 测试代码
[testing包](https://github.com/iteny/gopkg/tree/master/testing "点击进入")`(测试代码功能)`<br>



