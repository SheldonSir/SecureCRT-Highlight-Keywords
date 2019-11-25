# SecureCRT Highlight Keywords

在输入如
``` 
kubectl logs dash-7746bd789b-sckqk --all-containers=true 
``` 
之类的命令, 会向控制台输出很多数据, 每次都要定位到命令的开始部分, 有点浪费时间

我想高亮标记我输入的整行命令, 但SecureCRT Highlight Keywords 不能支持empty space, 所以只能标记输入命令的开始部分, 不是很完美, 但堪堪够用

![命令行高亮](./20191125122842.png)

```
// Edit Default Session -> Terminal -> Appearance -> Highlight Keywords, Append the follow Regular Expression
.+@.+:.*$
```
