# 使用手机当OBS直播摄像头-应用

B站：-诡锋丿Lavafall-

## 注意，部署时必须部署到使用https(http+ssl证书)的服务器中，不然获取摄像头模块无法正常工作，因为要保证链接的安全性

## 部署过程

1. 把npm run build打包的文件夹（我的是dist）推到github仓库

2. ~~~shell
   # dist是文件夹名，origin是远程git仓库的别名
   git subtree push --prefix dist origin gh-pages
   ~~~

   这样就可以自动在仓库创建一个gh-pages分支，并且自动部署到Github Pages

   如果不确定，就在仓库中的Settings里面看看pages的部署分支是否是gh-pages

3. 访问该应用即可：

   https://vincent-the-gamer.github.io/PhoneLiveCameraApp/