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

<table><thead>
<tr>
<th align="center">课时数</th>
<th align="left">课时标题</th>
<th align="left">在线播放</th>
</tr>
</thead><tbody>
<tr>
<td align="center">第 1 课</td>
<td align="left"><a href="/Unknwon/go-fundamental-programming/blob/master/lectures/lecture1.md">Go开发环境搭建</a></td>
<td align="left"><a href="http://www.tudou.com/programs/view/hlDq2A0vNes/">土豆网</a> <a href="http://www.ucai.cn/course/chapter/69/3210/4555">优才网</a> <a href="http://study.163.com/course/courseLearn.htm?courseId=306002#/learn/video?lessonId=421012&amp;courseId=306002">网易云课堂</a></td>
</tr>
</tbody>
</table>                         %
```
