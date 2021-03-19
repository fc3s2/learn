npm start
> [Node](https://nodejs.org/en/download/)
   
    npm -v
    node -v 
https://segmentfault.com/a/1190000023390756

    此处的环境配置主要配置的是 npm 安装的全局模块所在的路径，以及缓存cache的路径，之所以要配置，是因为以后在执行类似：npm install express [-g] （后面的可选参数-g，g代表global全局安装的意思）的安装语句时，会将安装的模块安装到【C:\Users\用户名\AppData\Roaming\npm】路径中，占C盘空间。
    例如：我希望将全模块所在路径和缓存路径放在我node.js安装的文件夹中，则在我的安装目录下创建两个文件夹【node_global】及【node_cache】如下图：

    设置环境变量 