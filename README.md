# One-paper 使用说明



### 效果预览图

![One-paper 预览图](https://raw.githubusercontent.com/zheli-design/hexo-theme-one-paper/main/source/img/one-paper-screenshot.jpg)



### 一些废话

这是一个真正「小而美」的主题，实话说，它应该叫做「skin」而不是「theme」，可这又有什么所谓呢 :-)

我不想把这个主题做成一个「大而全」的东西，它仅仅针对 **写作**，你也可以理解为是 **传统意义上的博客**。主要是以 **朴素干净轻量** 为主。

我在设计上花了一点心思，它的第一视觉效果是一张白纸，希望可以模拟在实体纸张阅读上的感受。今天它才是第一版本，后续迭代中，我会考虑让纸张更像纸张，比如，可以让白纸不是那么白，又或者，有点粗糙质感……

功能上我尽量与官方的靠齐，不新增额外非必要的功能（实际上是开发能力有限），后续慢慢研究，应该会把「常用」的一些功能补上。



### 支持

-   响应式设计，兼容手机端、pad 端以及 PC 端；
-   所有现代浏览器；
-   Markdown 支持的格式有限，目前仅做 `h1` ～ `h6`、文本、段落、表格等这些常用的；
-   功能上仅支持官方默认的，如导航菜单、分页等；
-   仅支持模版页：首页、文章详情页、归档页、单页；
-   无预留评论位置（后续可能会安排）。



### 安装

1.   下载 zip 压缩包并解压；
2.   Terminal 中 `Control + C` 停止 Hexo 服务；
3.   复制 one-paper 到 hexo\themes 目录下；
4.   更改 _config.yml 配置：`theme: one-paper`；
5.   `hexo s` 预览效果。



### 更改字体

主题内置了一个 [Google 字体 Montserrat](https://fonts.google.com/specimen/Montserrat)，如果不喜欢或有其他原因的，请删改以下内容：

-   layout\\_partial\head.ejs 中：

    ```
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,400;0,600;1,400;1,600&display=swap" rel="stylesheet">
    ```

-   source\css\style.css 中的 `Montserrat`：

    ```
    body
    {
        font-family: "Montserrat", "SF UI Text", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Segoe UI", "Helvetica Neue", Helvetica, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", sans-serif;
    }
    ```



### 更换 favicon

请同命名覆盖替换 source\img\favicon.png 图片。



### 其他

-   使用中遇到问题，可以在 [GitHub Issues](https://github.com/zheli-design/hexo-theme-one-paper/issues) 提交反馈；
-   如果你觉得主题不错，欢迎分享出去；
-   如果你熟悉 Hexo、Wordpress 等主题开发，正巧缺设计，也可以与我 [取得联系](https://zheli.design/contact.html)。



### 作者

[這Li](https://zheli.design/)



### 版权声明

遵守 [MIT License](https://zh.wikipedia.org/wiki/MIT許可證) 协议
