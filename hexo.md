[TOC]

# [**Hexo**](https://hexo.io/zh-cn/)

## 1. 安装Git
> [Git](https://gitforwindows.org/)
## 2. 安装Node.js
> [Node](https://nodejs.org/en/download/)
   
    npm -v
    node -v 
## 3. 安装Hexo
    新建文件夹,cd 到 新文件夹
    npm install -g hexo-cli
    hexo -v
    hexo init (可能遇到网络问题,多尝试或者取消代理)
    OpenSSL SSL_connect: SSL_ERROR_SYSCALL in connection
    git config --global --unset http.proxy
### 启动 
    hexo g
    hexo server (CTRL+C 终止)
    localhost:4000
## 4. 配置GitHub
    创建一个和GitHub同名的仓库 ***.github.io 
    测试连通性 ssh -T git@github.com
## 5. 发布文件到GitHub
    vscode中打开 第三步初始化的Hexo项目
    _config.yml deploy 
    type: git
    repo: https://github.com/YourgithubName/YourgithubName.github.io.git
    branch: master
    npm install hexo-deployer-git --save
    安装 deploy-git 也就是部署的命令
    
    hexo clean && hexo g && hexo d
    hexo clean
    hexo generate  hexo g
    hexo deploy  hexo d 注意deploy时可能要你输入username和password
    网络问题可能多次异常
    稍后即可访问 fc3s2.github.io

## 6.编写内容

## 7.设置域名(可选)
    现在你的个人网站的地址是 yourname.github.io，如果觉得这个网址逼格不太够，这就需要你设置个人域名了。但是需要花钱。

