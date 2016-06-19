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
[os包](https://github.com/iteny/gopkg/tree/master/os "点击进入")`(包以跨平台的方式，提供了一些与操作系统交互的函数和变量。程序的命令行参数可从os包的Args变量获取；os包外部使用os.Args访问该变量。)`<br>

# 数据库操作
[database/sql包](https://github.com/iteny/gopkg/tree/master/database/sql "点击进入")`(这是 Go 提供的操作 SQL/SQL-Like 数据库的通用接口，但 Go 标准库并没有提供具体数据库的实现，需要结合第三方的驱动来使用该接口。本书使用的是 mysql 的驱动：github.com/go-sql-driver/mysql。注：该包有一个子包：driver，它定义了一些接口供数据库驱动实现，一般业务代码中使用 database/sql 包即可，尽量避免使用 driver 这个子包。)`<br>

# 测试代码
[testing包](https://github.com/iteny/gopkg/tree/master/testing "点击进入")`(测试代码功能)`<br>

# 非安全类型操作
[unsafe包](https://github.com/iteny/gopkg/tree/master/unsafe "点击进入")`(一般被认为使用该库是不安全的。但是，在许多情况下，unsafe库的作用又是不可替代的，灵活地使用它们可以实现对内存的直接读写操作。在reflect库、syscall库以及其他许多需要操作内存的开源项目中都有对它的引用。)`<br>

# 并发相关
[sync包](https://github.com/iteny/gopkg/tree/master/sync "点击进入")`(处理同步需求)`<br>
[sync/atomic包](https://github.com/iteny/gopkg/tree/master/sync/atomic "点击进入")`(对于并发操作而言，原子操作是个非常现实的问题。典型的就是i++的问题。 当两个CPU同时对内存中的i进行读取，然后把加一之后的值放入内存中，可能两次i++的结果，这个i只增加了一次。 如何保证多CPU对同一块内存的操作是原子的。 golang中sync/atomic就是做这个使用的。)`<br>
[os/signal包](https://github.com/iteny/gopkg/tree/master/os/signal "点击进入")`(信号是事件发生时对进程的通知机制。有时也称之为软件中断。信号与硬件中断的相似之处在于打断了程序执行的正常流程，大多数情况下，无法预测信号到达的精确时间)`<br>





