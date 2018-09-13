<center>Nginx运行和控制</center>

# 1、nginx 命令行参数

查看nginx命令行参数，执行以下帮助命令。

```
nginx -h 
```

![1536810556269](images\帮助命令.png)

nginx执行的命令行参数，有上述10种，其各种参数分别表示什么含义，如下：

-？，-h   显示该帮助信息

-v            表示显示当前系统安装的nginx版本号。

![1536811045093](images\nginx-v.png)

-V             显示 nginx 的版本，编译器版本和配置参数。

![1536811377570](images\nginx-cmd-V.png)

-t              不运行，而仅仅测试配置文件。nginx 将检查配置文件的语法的正确性，并尝试打开配置文件中所引用到的文件。

-T               测试配置正确性，并且显示配置文件内容。

-q               测试配置时只显示错误。

-s                向主进程发送信号

                   - -  stop  停止nginx
                     -  quit   优雅的停止nginx
                     -  reload 重新加载配置文件
                     -  reopen 重新打开log文件

-p                设置nginx软件的安装路径

-c                 设置nginx配置文件

-g                 用于补充nginx配置，向nginx配置全局的指令。

​                     例如：>  nginx -g "pid /var/run/nginx.pid;"

​                      

# 2、nginx命令：启动，停止，重启

执行以下命令:

启动：

```
nginx
```

停止：

```
nginx -s stop
```

重启：

```
nginx -s reload 
```

