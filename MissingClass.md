# Shell和Bash
- Shell是用户和操作系统交互用的接口：能将计算机上的操作和指令翻译为二进制的命令传递给计算机内核。常见的shell有bash、sh、rsh、csh
- Bash是Ubuntu最常用的一种shell
- $0 脚本名 $1-9 脚本参数
- ！！ 完整的上一个命令
- $@ 所有参数
- false 返回 1 true 返回 0
- || 与 && 短路运算符
- 多个命令在同一行用；分割
```bash
  false; echo "This will always print"
  echo "we are in $(pwd)"
  cat <(ls) <(ls ..) #<(CMD)执行CMD并将结果输入到一个临时文件夹中 cat接收后面的内容
```
```bash
echo "hello"
ls 
mkdir project42
mkdir project1
ls project? #?一个字符
ls project* #*多个字符
convert image.png image.jpg
convert image.{png,jpg} #同样效果 {公共子串}

```
```bash
man CMD
CMD --help -h #了解命令的用法
```

```bash
find . -name src -type d
```