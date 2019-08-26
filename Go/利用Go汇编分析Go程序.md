利用汇编分析Go程序
===

## 查看方式
1.通过源码文件: go tool compile -S .\test.go(源码方式,以偏移量显示)
2.通过二进制文件: go tool objdump .\test.exe(反编译,会丢失部分信息)


## 命令详解
go tool compile -S filename  
比如我们有一个test.go的源文件,使用`go tool compile -S filename`即可查看对应的汇编指令集  
  
objdump  
用法:` go tool objdump [-S] [-s symregexp] binary [start end]`
比如我们有一个编译后的test.exe文件,我们可以使用`go tool objdump -S test.exe`来查看所有的汇编代码,或者使用**-s**参数来匹配部分代码,例如我们要查看main包下的test()方法:`go tool objdump -s "main\.test" test.exe`

## 资料补充
官网go汇编入门教程:https://golang.google.cn/doc/asm  
plan9汇编入门:https://xargin.com/plan9-assembly/  
go和plan9汇编:https://xargin.com/go-and-plan9-asm/  
go-internals中文版:https://github.com/go-internals-cn/go-internals  