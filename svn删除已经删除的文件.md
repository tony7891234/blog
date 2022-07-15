## 参考链接
- [https://blog.csdn.net/shengpeng3344/article/details/103621986](https://blog.csdn.net/shengpeng3344/article/details/103621986)


## 执行指令
`svn status | grep ! | awk '{print $2}' | xargs svn delete`
以上指令会将 所有!标识的变动变为D

## 解释
A | B 表示将A的输出给B

grep ! 表示过滤输入，输出所有带!的输出

xargs 表示获取每一个参数，然后对参数调用后面的命令。捕获一个命令的输出，然后传递给另外一个命令。 相当于svn delete 参数


## AWK文档
[https://awk.readthedocs.io/en/latest/chapter-one.html](https://awk.readthedocs.io/en/latest/chapter-one.html)
