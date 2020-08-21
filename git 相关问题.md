## ssh deploy key already in use

在部署GitHub项目出现这个问题，这个是因为某个项目引用了你的key，导致无法添加新的key到项目，解决方案：

通过以下指令查询到哪个项目使用了key，去删掉它
```
ssh -T -ai ~/.ssh/id_rsa git@github.com
```

然后在这个地方引用,重新添加
[https://github.com/settings/keys](https://github.com/settings/keys)