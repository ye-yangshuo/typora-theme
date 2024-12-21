# Type—Blue

## 前言：

最近在稀土掘金上发表文章，在编辑文章时发现稀土掘金中有个smart-blue的markdowm主题挺符合我的口味的。
因为我平时写文章都是在typora上写的，因此我就想把这个主题用在我的typora上。
我在github上找到了这个smart-blue主题的作者（[掘金markdown灵动蓝主题](https://github.com/cumt-robin/juejin-markdown-theme-smart-blue)）
当然这个主题不能直接在typora上调用，所以我对这个主题的css文件做了一定的修改，让这个主题适用于typora。

提示：以下链接都是学习时查阅的资料，整合起来方便查询。

## 调用：

[如何在typora中添加自定义CSS？ | typora中文网](https://www.typora.net/1765.html)

对基于typora的css文件，我们可以直接调用，以下为具体调用步骤：

1. 在文件中找到偏好设置：
   <img src="https://gitee.com/night-yangshuo/the-bed-of-pictures/raw/master/imgs/image-20241221105925580.png" alt="image-20241221105925580," style="zoom:50%;" />
2. 找到外观，点击打开主题文件夹，该文件夹存放css文件。
   **发现**：我在打开文件夹时发现，这个文件夹位于我的c盘，但我的typora安装在D盘。我在D盘中找到了与该主题文件夹一样的文件夹，然后我删除了C盘文件夹，再次进入typora后发现C盘的主题文件夹又生成了。
   **结论**：
   typora调用主题时会在C盘固定路径中寻找主题文件夹没有则生成；
   该文件夹是基于你的typora的真正存在位置的主题文件夹生成的；
   如果将css文件放在了真正typora所处的主题文件夹中，则无法调用该主题。
   <img src="https://gitee.com/night-yangshuo/the-bed-of-pictures/raw/master/imgs/1734750038726.png" alt="1734750038726，" style="zoom:50%;" />
3. 将css文件放入该文件夹，关闭并重新打开typora即可在主题中找到新放入的主题
   发现：我在控制台观察css调用情况时发现，怎么有文件加载失败。在搜索后我发现，原来是typora在调用css时有调用顺序：Typora 的基本样式——当前主题的 CSS——base.user.css ——{current-theme}.user.css 
   如果你的主题文件夹中不包含对应的css文件，在控制台就会报错，但基本不会影响主题调用。
   ![1734750772014](https://gitee.com/night-yangshuo/the-bed-of-pictures/raw/master/imgs/1734750772014.png)

至此主题调用成功

## 效果展示：

背景展示：

<img src="https://gitee.com/night-yangshuo/the-bed-of-pictures/raw/master/imgs/1734751324640.png" alt="1734751324640，" style="zoom:50%;" />

代码块展示：
	![1734751396684](https://gitee.com/night-yangshuo/the-bed-of-pictures/raw/master/imgs/1734751396684.png)

## 总结：

一个typora的蓝色系主题
如果对我的文章感兴趣：[夜阳朔 的个人主页 - 动态 - 掘金](https://juejin.cn/user/3248435137088570)
如果对主题感兴趣，可以下载下来自行探索。
最后**点个小小的star吧，嘤嘤嘤。**

