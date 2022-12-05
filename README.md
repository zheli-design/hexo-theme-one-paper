![One-paper 预览图](https://raw.githubusercontent.com/zheli-design/hexo-theme-one-paper/main/source/img/one-paper.png)



这是一个 [Hexo](https://hexo.io/) 主题，设计、开发于 2022 年 2 月。

这是一个「小而美」的主题，实话说，它应该叫做「skin」而不是「theme」，可这又有什么所谓呢 :-)

我不想把这个主题做成一个「大而全」的东西，它仅仅针对于 **写作**，你也可以理解为是 **传统意义上的博客**。主要是以 **朴素干净轻量** 为主。它的第一视觉效果是一张白纸，希望可以模拟在实体纸张阅读上的感受。

功能上尽量与官方的靠齐，非必要不新增。



### Live Demo

[https://zheli.design/one-paper](https://zheli.design/one-paper)



### 功能

-   响应式设计，兼容手机端、pad 端以及 PC 端；
-   支持所有现代浏览器；
-   Markdown 常用格式支持；
-   代码高亮、行数显示支持；
-   目前版本支持的模版页：首页、文章详情页、归档页、单页；
-   无预留评论位置（后续可能会安排）。



### 安装

1.   下载 zip 压缩包并解压；
2.   Terminal 中 `Control + C` 停止 Hexo 服务；
3.   复制 one-paper 到 hexo/themes 目录下；
4.   更改 _config.yml 配置：`theme: one-paper`；
5.   `hexo s` 预览效果。



### 内置第三方字体

主题内置了一个 [Google 字体 Montserrat](https://fonts.google.com/specimen/Montserrat)，如果不喜欢或有其他原因的，请删改以下三处内容：

1.   source/fonts 中的所有文件
2.   source/css/fonts.css
3.   source/css/style.css 中 line 21 的 `Montserrat`：

```css
body
{
    font-family: "Montserrat", "SF UI Text", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Segoe UI", "Helvetica Neue", Helvetica, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", sans-serif;
}
```



### 已开启高亮代码

主题内置了 [highlightjs](https://highlightjs.org/) 以及 [highlightjs-line-numbers.js](https://github.com/wcoder/highlightjs-line-numbers.js) 两个插件，默认启用，无需手动开启。如无效果，请将 hexo/_config.yml 中的以下两处 `true` 改为 `false`：

```yml
highlight:
  enable: false
prismjs:
  enable: false
```



### 更换 favicon

请同命名覆盖替换 source/img/favicon.png 图片。

### 添加公式渲染功能

1. 首先执行以下命令卸载掉hexo默认的渲染插件`hexo-renderer-marked` ，替换为`hexo-renderer-markdown-it-plus` 。

    ```C++
    npm un hexo-renderer-marked --save
    npm i hexo-renderer-markdown-it-plus --save
    ```

2. 修改`hexo_root/scaffolds/post.md` 文件，在末尾添加一行 `math: true`。

    之后当你执行`hexo new title`生成一篇新的文章时，文章内部默认配置如下所示：
    ![20220616213508](https://s2.loli.net/2022/06/16/qt5NvLhundmMoce.png)

    这样公式渲染默认是开启的，我们直接编写文章正文即可，如果想关闭数学公式支持，将`true`修改为`false`即可。
    
3. 在`根目录下`配置站点配置文件 `_config.yml`，在最后面加入如下配置：

    ```C++
    markdown_it_plus:
      highlight: true
      html: true
      xhtmlOut: true
      breaks: true
      langPrefix:
      linkify: true
      typographer:
      quotes: “”‘’
      pre_class: highlight
    ```

### 其他

-   如果你觉得主题不错，欢迎分享出去；使用中遇到问题，可以在 [GitHub Issues](https://github.com/zheli-design/hexo-theme-one-paper/issues) 提交反馈；
-   如果你熟悉 Hexo、Wordpress 主题开发，正巧缺设计，也可以与我 [取得联系](https://zheli.design/)。



### 作者

[這李設計](https://zheli.design/)



### 版权声明

遵守 [MIT License](https://zh.wikipedia.org/wiki/MIT許可證) 协议
