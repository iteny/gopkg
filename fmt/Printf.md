
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
		<th align="center" width="20">占位符</th>
		<th align="left" width="30">说明</th>
		<th align="left" width="30">举例</th>
		<th align="left" width="20">输出</th>
	</tr>
	</thead>
	<tbody>
	<tr>
		<td align="center">%v</td>
		<td align="left">相应值的默认格式。</td>
		<td align="left">Printf("%v", site)，Printf("%+v", site)</td>
		<td align="center">{iteny}，{Name:iteny}</td>
	</tr>
	</tbody>
</table>                         

