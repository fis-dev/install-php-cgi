各种系统环境下安装php-cgi的方法
------------

## \*nix一键安装php-cgi环境

```shell
cd ~
bash -c "$( curl http://fouber.github.io/install-php-cgi/install-php.sh -k )" -o 5.3.5
```

说明：

* cd到一个合适的目录，脚本会在该目录下创建一个 ``php-linux`` 目录，在此目录内安装
* 安装的最后阶段，会执行 ``sudo ln -s php-linux/bin/php-cgi /usr/local/bin/php-cgi`` 命令，旨在用户可以直接执行 ``php-cgi``，这一步可以取消，用户自行处理。 
* ``-o 5.3.5`` 参数表示安装php的 ``5.3.5`` 版本，此参数可省略，默认安装的版本是 ``5.2.17``
