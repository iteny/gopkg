
# func Printf(format string, a ...interface{}) (n int, err error)

参数列表

- format 打印的格式说明 
- a... 值变量列表

返回值：

- 返回打印字符数 n
- 返回error

功能说明：

这个函数主要是用来根据说明格式字符串和参数表生成一个打印字符串

代码实例：

 	package main
	
	import 	"fmt"
		
	func main() {
		fmt.Printf("Format:%s\n","格式打印!")
	}
```
type Website struct {
    Name string
}

// 打印结构体时
var site = Website{Name:"iteny"}
```
# 普通占位符
<table>
	<thead>
	<tr>
		<th align="center" width="10%">占位符</th>
		<th align="left" width="30%">说明</th>
		<th align="left" width="30%">举例</th>
		<th align="left" width="30%">输出</th>
	</tr>
	</thead>
	<tbody>
	<tr>
		<td align="center">%v</td>
		<td align="left">变量的自然形式(natural format),在打印结构体时,“加号”标记(%+v)会添加字段名</td>
		<td align="left">Printf("%v", site)，Printf("%+v", site)</td>
		<td align="left">{iteny}，{Name:iteny}</td>
	</tr>
	<tr>
		<td align="center">%#v</td>
		<td align="left">变量的Go语法表示</td>
		<td align="left">Printf("#v", site)</td>
		<td align="left">main.Website{Name:"iteny"}</td>
	</tr>
	<tr>
		<td align="center">%T</td>
		<td align="left">变量的类型</td>
		<td align="left">Printf("%T", site)</td>
		<td align="left">main.Website</td>
	</tr>
	<tr>
		<td align="center">%%</td>
		<td align="left">字面上的百分号标志(并非值的占位符)</td>
		<td align="left">Printf("%%")</td>
		<td align="left">%</td>
	</tr>
	</tbody>
</table>                         

# 布尔占位符
<table>
	<thead>
	<tr>
		<th align="center" width="10%">占位符</th>
		<th align="left" width="30%">说明</th>
		<th align="left" width="30%">举例</th>
		<th align="left" width="30%">输出</th>
	</tr>
	</thead>
	<tbody>	
	<tr>
		<td align="center">%t</td>
		<td align="left">布尔：true或false</td>
		<td align="left"> Printf("%t", true)</td>
		<td align="left">true</td>
	</tr>
	</tbody>
</table>   

# 整数占位符
<table>
	<thead>
	<tr>
		<th align="center" width="10%">占位符</th>
		<th align="left" width="30%">说明</th>
		<th align="left" width="30%">举例</th>
		<th align="left" width="30%">输出</th>
	</tr>
	</thead>
	<tbody>	
	<tr>
		<td align="center">%b</td>
		<td align="left">二进制表示</td>
		<td align="left">Printf("%b", 5)</td>
		<td align="left">101</td>
	</tr>
	<tr>
		<td align="center">%c</td>
		<td align="left">相应Unicode码点所表示的字符</td>
		<td align="left">Printf("%c", 0x4E2D)</td>
		<td align="left">中</td>
	</tr>
	<tr>
		<td align="center">%d</td>
		<td align="left">十进制表示</td>
		<td align="left">Printf("%d", 0x12)</td>
		<td align="left">18</td>
	</tr>
	<tr>
		<td align="center">%o</td>
		<td align="left">八进制表示</td>
		<td align="left">Printf("%d", 10)</td>
		<td align="left">8</td>
	</tr>
	<tr>
		<td align="center">%q</td>
		<td align="left">单引号围绕的字符字面值，由Go语法安全地转义</td>
		<td align="left">Printf("%q", 0x4E2D)</td>
		<td align="left">'中'</td>
	</tr>
	<tr>
		<td align="center">%x</td>
		<td align="left">十六进制表示，字母形式为小写 a-f</td>
		<td align="left">Printf("%x", 13)</td>
		<td align="left">d</td>
	</tr>
	<tr>
		<td align="center">%X</td>
		<td align="left">十六进制表示，字母形式为大写 A-F</td>
		<td align="left">Printf("%x", 13)</td>
		<td align="left">D</td>
	</tr>
	<tr>
		<td align="center">%U</td>
		<td align="left">Unicode格式：U+1234，等同于 "U+%04X"</td>
		<td align="left">Printf("%U", 0x4E2D)</td>
		<td align="left">U+4E2D</td>
	</tr>
	</tbody>
</table>   

# 浮点数和复数的组成部分(实部和虚部)
<table>
	<thead>
	<tr>
		<th align="center" width="10%">占位符</th>
		<th align="left" width="30%">说明</th>
		<th align="left" width="30%">举例</th>
		<th align="left" width="30%">输出</th>
	</tr>
	</thead>
	<tbody>	
	<tr>
		<td align="center">%e</td>
		<td align="left">科学计数法，例如 -1234.456e+78</td>
		<td align="left"> Printf("%e", 10.2)</td>
		<td align="left">1.020000e+01</td>
	</tr>
	<tr>
		<td align="center">%E</td>
		<td align="left">科学计数法，例如 -1234.456E+78</td>
		<td align="left">Printf("%E", 10.2)</td>
		<td align="left">1.020000E+01</td>
	</tr>
	<tr>
		<td align="center">%f</td>
		<td align="left">有小数点而无指数，例如 123.456</td>
		<td align="left">Printf("%f", 10.2)</td>
		<td align="left">10.200000</td>
	</tr>
	<tr>
		<td align="center">%g</td>
		<td align="left">根据情况选择 %e 或 %f 以产生更紧凑的（无末尾的0）输出</td>
		<td align="left">Printf("%g", 10.20)</td>
		<td align="left">10.2</td>
	</tr>
	<tr>
		<td align="center">%G</td>
		<td align="left">根据情况选择 %E 或 %f 以产生更紧凑的（无末尾的0）输出</td>
		<td align="left">Printf("%G", 10.20+2i)</td>
		<td align="left">(10.2+2i)</td>
	</tr>	
	</tbody>
</table>

# 字符串与字节切片
<table>
	<thead>
	<tr>
		<th align="center" width="10%">占位符</th>
		<th align="left" width="30%">说明</th>
		<th align="left" width="30%">举例</th>
		<th align="left" width="30%">输出</th>
	</tr>
	</thead>
	<tbody>	
	<tr>
		<td align="center">%s</td>
		<td align="left">输出字符串表示（string类型或[]byte)</td>
		<td align="left">Printf("%s", []byte("Go语言学习园地"))</td>
		<td align="left">Go语言学习园地</td>
	</tr>
	<tr>
		<td align="center">%q</td>
		<td align="left">双引号围绕的字符串，由Go语法安全地转义</td>
		<td align="left">Printf("%q", "Go语言学习园地")</td>
		<td align="left">"Go语言学习园地"</td>
	</tr>
	<tr>
		<td align="center">%x</td>
		<td align="left">十六进制，小写字母，每字节两个字符</td>
		<td align="left">Printf("%x", "golang")</td>
		<td align="left">676f6c616e67</td>
	</tr>
	<tr>
		<td align="center">%X</td>
		<td align="left">十六进制，大写字母，每字节两个字符</td>
		<td align="left">Printf("%X", "golang")</td>
		<td align="left">676F6C616E67</td>
	</tr>
	</tbody>
</table> 

# 指针
<table>
	<thead>
	<tr>
		<th align="center" width="10%">占位符</th>
		<th align="left" width="30%">说明</th>
		<th align="left" width="30%">举例</th>
		<th align="left" width="30%">输出</th>
	</tr>
	</thead>
	<tbody>	
	<tr>
		<td align="center">%p</td>
		<td align="left">十六进制表示，前缀 0x</td>
		<td align="left">Printf("%p", &site)</td>
		<td align="left">0x4f57f0</td>
	</tr>
	</tbody>
</table> 

# 其他占位符
<table>
	<thead>
	<tr>
		<th align="center" width="10%">占位符</th>
		<th align="left" width="30%">说明</th>
		<th align="left" width="30%">举例</th>
		<th align="left" width="30%">输出</th>
	</tr>
	</thead>
	<tbody>	
	<tr>
		<td align="center">+</td>
		<td align="left">总打印数值的正负号:对于%q(%+q)保证只输出ASCII编码的字符。</td>
		<td align="left">Printf("%+q", "中文")</td>
		<td align="left">"\u4e2d\u6587"</td>
	</tr>
	<tr>
		<td align="center">-</td>
		<td align="left">在右侧而非左侧填充空格(左对齐该区域)</td>
		<td align="left"></td>
		<td align="left"></td>
	</tr>
	<tr>
		<td align="center">#</td>
		<td align="left">备用格式:为八进制添加前导0(%#o)，为十六进制添加前导0x(%#x)</td>
		<td align="left">Printf("%#U", '中')</td>
		<td align="left">U+4E2D '中'</td>
	</tr>
	<tr>
		<td align="center">' '</td>
		<td align="left">(空格)为数值中省略的正负号留出空白(% d)</td>
		<td align="left"></td>
		<td align="left"></td>
	</tr>
	<tr>
		<td align="center">0</td>
		<td align="left">填充前导的0而非空格:对于数字,这会将填充移到正负号之后</td>
		<td align="left"></td>
		<td align="left"></td>
	</tr>
	</tbody>
</table> 






