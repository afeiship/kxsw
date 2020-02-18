# http-ssh-propxy

## git 设置和取消代理(http/https)
- https://gist.github.com/laispace/666dd7b27e9116faece6
- https://gist.github.com/chuyik/02d0d37a49edc162546441092efae6a1

## ssh proxy
- https://www.mikeheijmans.com/sysadmin/2014/08/12/proxy-ssh-over-socks/

~~~
对于使用git@协议的，可以配置socks5代理
在~/.ssh/config 文件后面添加几行，没有可以新建一个

Host github.com
ProxyCommand nc -X 5 -x 127.0.0.1:1080 %h %p
~~~
