git 冲突

cd ~/.ssh
ls -al ~/.ssh

cd ~/.ssh
ll | ls

ssh-keygen -t rsa -C "******@gmail.com"
cat id_rsa.pub

ssh -T git@github.com

> OpenSSL SSL_connect: SSL_ERROR_SYSCALL in connection

git config --global --unset http.proxy

## git名字检查 | 修改
    git config user.name
    git config user.email
    git config --global user.name "yourname"
    git config --global user.email "youremail"

