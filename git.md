### 生成密匙
- 检查是否已经有了ssh密匙
cd ~/.ssh
如果没有密钥则不会有此文件夹，有则备份删除，一般是在C盘当前用户里面的.ssh文件夹内

- 设置Git的user name和email：
```
$ git config --global user.name "xxx"
$ git config --global user.email "xxx@xx.com"
```

- 生成SSH密钥过程：
$ ssh-keygen -t rsa -C “xxx@xx.com”   
按3个回车，密码为空。   
最后得到了两个文件：id_rsa和id_rsa.pub   
在github上添加ssh密钥，这要添加的是“id_rsa.pub”里面的公钥。

### TortoiseGit 
- 第一次提交记住账户和密码
在C:\Documents and Settings\Administrator\ 目录下有一个  .gitconfig 的文件，里面会有你先前配好的name 和email，只需在下面加一行
```
[credential] 
helper = store
```


