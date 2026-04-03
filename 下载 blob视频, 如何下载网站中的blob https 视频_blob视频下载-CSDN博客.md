# 下载 blob视频, 如何下载网站中的blob:https:// 视频_blob视频下载-CSDN博客
转载 于 2020-10-17 08:50:49 发布 · 10w+ 阅读

· ![](https://csdnimg.cn/release/blogv2/dist/pc/img/newHeart2023Black.png)
 27 

· ![](https://csdnimg.cn/release/blogv2/dist/pc/img/tobarCollect2.png)
  123   ·

方法一：手机模式查连接
-----------

![](https://i-blog.csdnimg.cn/blog_migrate/c27f32e9cf76b952a4f8a9570c199dd9.png)

![](https://i-blog.csdnimg.cn/blog_migrate/95709bf59602885d3f29666af51d731b.png)

方法二：Blob格式视频下载
--------------

1，引入
----

1，在网页中，如果看到自己喜欢的视频，想下载下来，在 控制台 一步步的找到这个元素之后，发现格式是 `blob`格式的，就很尴尬， 下面详细介绍如何进行下载。

![](https://i-blog.csdnimg.cn/blog_migrate/b88fc995c899dc3e715a344d13c46f87.png)

下载 blob视频, 如何下载网站中的blob:https:// 视频

2，步骤
----

2.1，打开控制台

在`NetWork`这一栏，对请求进行通过关键词`.m3u8`进行过滤，过滤的结果中，某一个请求的url是以`.m3u8`结束的，

> 现在就从下载 Blob 格式的转为下载 m3u8 格式的了。

![](https://i-blog.csdnimg.cn/blog_migrate/de08149972a4607d515cf297edb402ae.png)

下载 blob视频, 如何下载网站中的blob:https:// 视频

### 2.2，m3u8格式的下载

#### 2.2.1， ffmpeg 工具下载

> 使用这个工具下载 m3u8，是因为最简单。 [这是ffmpeg的官网](https://link.juejin.im/?target=https%3A%2F%2Fffmpeg.zeranoe.com%2Fbuilds%2F)

1，点击下面进行下载：

![](https://i-blog.csdnimg.cn/blog_migrate/587fb5f4e9f241579595a11de39510d8.png)

下载 blob视频, 如何下载网站中的blob:https:// 视频

2，下载的是一个压缩文件，解压后会有如下的文件夹。

![](https://i-blog.csdnimg.cn/blog_migrate/d7526b1312c996aedee359d5412756af.png)

下载 blob视频, 如何下载网站中的blob:https:// 视频

3，将上面的所有文件copy到一个文件夹中（注意命名为英文），下面是我的目录

![](https://i-blog.csdnimg.cn/blog_migrate/f2c0371b5a201b740bc290da9c0c356c.png)

下载 blob视频, 如何下载网站中的blob:https:// 视频

4， 配置环境 变量将上面目录添加为环境变量。

5，检查是否成功

在 命令行 中输入 `ffmpeg -verison`

出现下面的情况，说明`ffmpeg`安装成功

![](https://i-blog.csdnimg.cn/blog_migrate/99231a60f61003d80198bba79487cf3e.png)

下载 blob视频, 如何下载网站中的blob:https:// 视频

#### 2.2.2，下载

| `1` | `ffmpeg -i 链接 目标文件.mp4（也可以是其他视频格式）` |

#### 更加详细的使用可以看 [百度百科](https://link.juejin.im/?target=https%3A%2F%2Fbaike.baidu.com%2Fitem%2Fffmpeg%2F2665727%3Ffr%3Daladdin)

eg：下载上面哪个视频的的话

| `1` | `ffmpeg -i https:``//video``.[twimg.com](http://twimg.com/)``/ext_tw_video/1143530317296406529/pu/pl/720x720/69ZLvxR5w_0y7mVj``.m3u8 demo.mp4` |

**2.2.3，下载目录**

这个直接在电脑上进行搜索 文件名 即可，推荐使用everything这个工具，[官网下载地址](https://link.juejin.im/?target=https%3A%2F%2Fwww.voidtools.com%2Fzh-cn%2F)