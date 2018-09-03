# 调试node配置
http://www.cnblogs.com/answercard/p/6125473.html

上面的文章一般调试node的步骤，但是我曾经遇到有个项目，要运行的node的配置文件在项目文件夹根目录里面的子文件夹
![](http://oys6fh33c.bkt.clouddn.com/QQ%E5%9B%BE%E7%89%8720171102161055.png)

在点击调试按钮时没法自动检测到back-end里面的app.js，所以要在根目录下新建“.vscode”文件，再新建launch.json文件，改好路径即可
![](http://oys6fh33c.bkt.clouddn.com/20171102161505.png)

# vscode 不同两台电脑，插件保存（setting sync）

需要拿到两个参数：
token和gist id

详细获取步骤可参考这个：
[Atom 备份神器 —— Sync Settings](http://www.cnblogs.com/hooray/p/5885211.html "Atom 备份神器 —— Sync Settings")  

遇到的问题：  
- https://gist.github.com 无法打开
修改host：204.232.175.94 http://gist.github.com
- 插件报错:  
https://segmentfault.com/q/1010000008183902  
https://segmentfault.com/a/1190000011206401  

一般报错先重置插件的配置，或者跟新token即可
