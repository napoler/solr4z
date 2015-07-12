# Solr4Z #
Apache solr handy package, ALL in ONE package.
> startup utilities,
> Jetty,
> Solr,
> IKAnalyzer,
> Drupal6/Drupal7 Supported.

Solr快捷包，包含Solr的启动关闭脚本，中文配置等。
Jetty, IKAnalyzer, Drupal6/Drupal7配置切换，一键启动。

```
./solrd start [start]
./solrd stop  [stop]
./solrd startx [start as front process]
./solrd switch 6 [switch to drupal6 schema] (beta2)
./solrd switch 7 [switch to drupal7 schema] (beta2)
./solrd clean [clean up the data and log] (beta2)
```

**启动之后打开浏览器，输入http://localhost:8993/solr**

详情说明以及更新说明，会在本人博客上陆续更新，请参考：
[Drupal与高性能网站架构](http://www.drupal001.com)

**上面的管理命令，仅支持Linux/Unix，若要支持windows，请自行修改文件里面对应的软连接（solr/conf/里面），以及solrd脚本。**


---

### Windows版本Drupal7+中文支持Solr包 ###

请下载 solr4z\_3.6.1\_ik2012\_d7.tar.gz ，然后解压缩。

在windows下面打开命令行工具，（运行里面输入 cmd）
使用cd命令进入当前目录，比如
```
cd solr4z_3.6.1_ik2012_d7
```
最终的启动服务器代码：

```
java -jar start.jar
```
即可启动了服务器。

然后在浏览器里，输入http://localhost:8993/solr 查看solr的管理界面。

PS：还有一种简单的办法，进入solr目录，双击start.jar看看能否启动成功，浏览器打开 http://localhost:8993/solr 查看。

---


PS: Drupal 添加自定义字段到Solr推荐使用模块
[ApacheSolr Custom Fileds](http://drupal.org/project/apachesolr_custom_fields)