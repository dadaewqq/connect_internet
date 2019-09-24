# 《这本书能让你连接互联网 Ⅱ》


## ***intro***

本书着重于上网的方式与获取信息的技巧，并对相关流行且典型的软件做简要的上手配置，以及原理的相关说明。



[导读](docs/README.md)--------------------------------------------[目录](docs/_sidebar.md)---------------------------------------------------[后记](docs/postscript.md)



**《这本书》示例的多数网址，以及更多资料收录在 [WebSiteOutlook](https://github.com/hoodiearon/WebSiteOutlook) ，书中的相关章节搭配存储库 `科学上网` 效果会更好！**

## ***update***

《这本书能让你连接互联网》-> 《这本书能让你连接互联网 Ⅱ》的更新要点：

* 增加速成科学上网篇章
* 增加相关上网方式以及软件配置操作
* crx_header_invalid 解决方案的说明
* VPN连接上服务器却无法访问任何网页及其他网络的解决办法
* Windows 无法设置系统代理的问题
* 项目内置 probot 机器人，method 新增 战略家模式

* <details><summary>其他更新 click me! </summary>

    * 增加对虚拟电话注册方案的说明
    * 谷歌新账户注册方式
    * 网页时光机以及查找相似站点
    * 利用个人博客作为连接互联网的中转

    </details>

此外，还精简了不必要的重复内容，图片采用 postimages 支持，项目由30M降低到144KB大小，非常方便在线部署及下载，欢迎 fork 《这本书》！

## ***usage***



### 在线部署

1. fork 《这本书》 到你的 repo
2. 修改 docs/index.html 将`window.$docsify = {}` 的`repo` 修改成你的 repo
3. 在 settings 找到 GitHub Pages 并选择 `master brach/docs folder` 
4. 访问 `https://你的GitHub用户名.github.io/how_network_works_book` 即可看到效果



### 本地部署

所需环境：[git](https://git-scm.com/)、[node](https://nodejs.org/zh-cn)；安装很简单一直 `下一步` 直到完成安装即可。

* 右击选择`git bash`在命令行中输入 `npm i docsify-cli -g`
* 点击`clone or download`下载`.zip` 并解压缩
* 进入到`how_network_works_book-master/docs`目录
* 右击打开`git bash`输入`docsify init .`
* 使用`docsify serve`完成本地部署
* 在浏览器中输入`localhost:3000`即可看到效果 :joy: 

关于更多详细，请看[docsify官网文档](https://docsify.js.org/)

当然，也可使用[wkhtmltopdf](https://github.com/wkhtmltopdf/wkhtmltopdf)  以及结合[tools.pdf24.org](https://tools.pdf24.org/zh/webpage-to-pdf)制作《这本书》的PDF



### 获取更新

以01user为例，在本地部署时，旧版图链已经失效了，Ⅱ版已经采用 postimage 支持；此时就需升级成 《这本书Ⅱ》,获取更新其实非常简单，在fork的基础上，执行以下指令

```
git clone https://github.com/你的github用户名/how_network_works_book.git
cd 
git remote add upstream https://github.com/hoodiearon/how_network_works_book.git
# 若需必要的分支变更，还是使用合适： git fetch --all
git fetch upstream
# 对Git有所了解的话，建议还是使用：`git pull upstream master --allow-unrelated-histories` 以审查代码的形式更新
git reset --hard upstream/master

```
提交到自己的repo

```
git add .
git commit -m "test"
# 此指令只方便newbie或不得已的强制；会些Git还是推荐：git push -u --force-with-lease origin master
git push -u -f origin master  
```

输入账号&密码即可上传到自己repo完成Github账户仓库远程更新。



## ***mind you*** 

本书允许演绎及共享但禁止商用，科学上网仅为研究需要，以下是免责声明：

* 本书面向海外华人用户且仅供科研与学习，切勿用于其他用途
* 中国居民请自觉关闭本书并24小时内删掉与此相关的所有内容，否则出现一切后果本书作者概不负责

© 2019 [hoodiearon](https://github.com/hoodiearon)



