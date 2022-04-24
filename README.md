# Hexo-file

##  目录

*   [关于](#关于)

    *   [What is it?](#what-is-it)

    *   [为什么不用](#为什么不用)

    *   [有什么缺陷](#有什么缺陷)

    *   [''我''怎么使用？](#我怎么使用)

        *   [把文件全部下载下来](#把文件全部下载下来)
        *   [修改 hexo-bb 配置](#修改-hexo-bb-配置)
        *   [更改评论系统](#更改评论系统)

    *   [随机封面](#随机封面)

    *   [其它](#其它)

# 关于

## What is it?

这是我以前 Hexo 博客配置，但是最后不用了。

本配置采用 [\*\* hexo-theme-stellar 1.7.0\*\*](https://github.com/xaoxuu/hexo-theme-stellar " hexo-theme-stellar 1.7.0")

在原来的基础上 ，增加了 ”一言“ "[说说](https://www.npmjs.com/package/hexo-bb "说说")" 等

在 hexo: 5.4.2，hexo-cli: 4.3.0，node: 16.13.1 上正常部署

## 为什么不用

我在配置过程中，多次被其他事情影响，导致配置过程缓慢，到最后就是搞一点忘一点，报错数次之后也懒得用了。

另外就是这个主题并不支持搜索（但它是针对专栏的博客）

## 有什么缺陷

*   \[ ]   BB与专栏界面导航栏未能变灰色

     ![](https://cdn.jsdelivr.net/gh/RamSong/before-blog-file@main/3.png)

*   \[ ] sitemap不能正常显示（去看文档应该就行了，我懒）

    ![](https://cdn.jsdelivr.net/gh/RamSong/before-blog-file@main/2.png)

    其它问题暂未发现

## ''我''怎么使用？

Star一下（doge）

### 把文件全部下载下来

### 修改 hexo-bb 配置

在 \_config.yml 下

```yaml
bb:
 title: Ram动态  #页面title
 appId: 哈哈哈哈
 appKey: 哈哈哈哈
 serverURLs: 自己填啊 #你的api地址
 limit: 15 #显示条数
 path: bb #路径名称 例如：https://127.0.0.1/bb
 content: '👉🏼此说说对接腾讯服务，通过📱微信发出，相当于一个QQ说说。📑' #显示在哔哔上方,如不需要注释即可
```

把 title，appid，appkey，serverURLs 改成你自己的

可参考其 [**官方文档**](https://www.npmjs.com/package/hexo-bb "官方文档")

### 更改评论系统

在 \_config.stellar.yml 下

```yaml
comments:
  service: beaudar # beaudar, utterances, valine, twikoo
  # beaudar
  # https://beaudar.lipk.org/
  beaudar:
    repo: 改成你的
    issue-term: pathname
    issue-number:
    theme: preferred-color-scheme
    label:
    input-position: top # top/bottom 评论框位置
    comment-order: desc # desc 排序
    keep-theme: # true/false
    loading: false
    branch: main
```

更改 service 即更改评论系统

我使用的是 Beaudar评论系统，如果你也想用，参考 [**官方文档**](https://beaudar.lipk.org/ "官方文档") 配置Github仓库安装插件后，把repo改成你的即可

这个评论系统还是可以的（还有很多主题）：

![](https://cdn.jsdelivr.net/gh/RamSong/before-blog-file@main/1.png)

## 随机封面

主题自带的随机封面太正经了

这里推荐几个二次元API

只需在文章头部插入即可：

![](https://cdn.jsdelivr.net/gh/RamSong/before-blog-file@main/4.png)

1.  [https://api.lqbby.com/api/dm](https://api.lqbby.com/api/dm "https://api.lqbby.com/api/dm")

2.  [https://api.ghser.com/random/api.php](https://api.ghser.com/random/api.php "https://api.ghser.com/random/api.php")

3.  [https://img.xjh.me/random\_img.php?return=302](https://img.xjh.me/random_img.php?return=302 "https://img.xjh.me/random_img.php?return=302")

4.  [https://api.ixiaowai.cn/api/api.php](https://api.ixiaowai.cn/api/api.php "https://api.ixiaowai.cn/api/api.php")

5.  [https://img.paulzzh.com/touhou/random](https://img.paulzzh.com/touhou/random "https://img.paulzzh.com/touhou/random")

6.  [https://tuapi.eees.cc/api.php?category=dongman\&type=302](https://tuapi.eees.cc/api.php?category=dongman\&type=302 "https://tuapi.eees.cc/api.php?category=dongman\&type=302")

7.  [https://api.ishimeng.cn/ecy/api.php](https://api.ishimeng.cn/ecy/api.php "https://api.ishimeng.cn/ecy/api.php")

8.  [https://api.codeanime.cn/4kanimation/random.php（4k动漫）](https://api.codeanime.cn/4kanimation/random.php） 

够你用几年了把（doge）

## 其它

一些别的配置请参考 [**hexo-theme-stellar文档**](https://xaoxuu.com/wiki/stellar/ "hexo-theme-stellar文档") 中的教程进行配置

有什么问题也可以和它的作者留言

其实这是一个很好的主题，只不过它尚在孩童阶段，希望作者能加紧更新
