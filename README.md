# Analytics Dashboard

<a href="https://paradiseeee.github.io/AnalyticsDashboard" target="_blank">
  <img src="./readme-assets/github-mirror.svg" style="max-width:100%;">
</a>
<a href="https://paradiseeee.gitee.io/AnalyticsDashboard" target="_blank">
  <img src="./readme-assets/gitee-mirror.svg" style="max-width:100%;">
</a>

## 结构简介

本仓库为本人创建的一个数据分析项目展示网站模版，主要包括一下内容：

- 数据集的概要信息
    - 对数据集整体信息的可视化图表
    - 对数据集的描述统计分析信息
- 细分领域的分析
    - 主要为对不同分类的横向或纵向对比，类似 Excel 的数据透视表的功能
- 数据挖掘和建模分析
    - 针对关注的问题进行建模分析，并可视化结果
- 数据源和代码
    - 项目中用到的数据集和数据分析代码等资源

## 开发过程

由于本人并没有系统地学过前端知识，仅是凭着一个好玩的想法就动手做了，所以实际做出来的知识一个静态的展示网页，没有后端数据库也没有动态更新的功能。

首先是寻找一个好看的网页模版，这里只需要用到基本的网页结构，例如 **css** 布局，**UI** 元素等。这个很多地方都能找到合适的，不再赘述。

接下来就是确定要展示的内容，然后调整网页模版以适应展示的内容。在开发的过程中由于都是拍脑袋修改的，很多视觉效果上的代码都是直接在 **HTML** 上改的，没有去整合到 **css**。最后做出来也懒得改了，就这样了。

搞定布局后就可以在上面堆砌图表了，这里用的是 **ECharts**，虽然功能一般，但是比较简单，而且有 **Python** 的库支持，可以很容易地整合到数据处理的流程里，批量地生成可视化图表。

在完成的网页中，有分组分析的内容。由于网页内容高度相似，这里就用 **vue** 和 **jquery** 来实现更新网页，减少源码的冗余度。注意到代码和数据的网页是直接用了多个 **HTML** 文档作为不同的标签页，因为这是一开始写的，后来才发现这样写太愚蠢了，但是又懒得改回来了。

关于**复用**的问题，暂时目测这个模版要拿来复用是够呛的，除非是高度相似的数据分析项目。例如同一个主题不同时间节点的分析展示，或同一个数据集不同侧重点的分析展示。所以结论就是，没有什么复用的价值。但是进一步整理一下感觉还是*有救的*。

注意到网页上展示的内容都是由 **Python** 生成的，数据处理和分析建模的过程也是使用 **Python** 完成的。

------------------------

~~你还别说，虽说没啥用但还挺好玩！~~