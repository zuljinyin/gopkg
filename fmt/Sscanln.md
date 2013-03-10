# func Sscanln(str string, a ...interface{}) (n int, err error)

参数列表

- str 指定源字符串
- a... 值变量列表

返回值：

- 返回成功读取的参数的数量 n
- 返回error

功能说明：

>这个函数主要是从指定源字符串str中读取文本，将空白分割的连续数据顺序存入参数里。
>
>换行视同空白。它返回成功读取的参数的数量。
>
>如果少于提供的参数的数量，返回值err将报告原因。
>
>类似Scan，但会在换行符中止，并且存入最后一条后时读取位置必须有换行或者结束符。

代码实例：

        package main

        import  "fmt"

        func main(){
        	str := "34  343  245"
                var a,b,c int
                fmt.Sscanln(str,&a,&b,&c)
                fmt.Println(a,b,c)
        }

