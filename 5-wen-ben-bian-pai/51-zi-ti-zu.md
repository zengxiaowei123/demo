#### \[强制\] font-family 属性中的字体族名称应使用字体的英文 Family Name，其中如有空格，须放置在引号中。

解释：

所谓英文 Family Name，为字体文件的一个元数据，常见名称如下：

| **字体** | **操作系统** | **Family Name** |
| :---: | :---: | :---: |
| 宋体（中易宋体） | windows | SimSun |
| 黑体（中易黑体） | windows | SimHei |
| 微软雅黑 | windows | Microsoft YaHei |
| 微软正黑 | windows | Microsoft JhengHei |
| 华文黑体 | mac/ios | STHeiti |
| 冬青团体 | mac/ios | Hiragino Sans GB |
| 文泉驿正黑 | linux | WenQuanYi Zen Hei |
| 文泉驿微米黑 | linux | WenQuanYi Micro Hei |

示例：

h1 {

    font-family: "Microsoft YaHei";

}

#### \[强制\] font-family 按「西文字体在前、中文字体在后」、「效果佳 \(质量高/更能满足需求\) 的字体在

#### 前、效果一般的字体在后」的顺序编写，最后必须指定一个通用字体族\( serif /sans-serif \)。

解释：

更详细说明可参考本文。

示例：

/\* Display according to platform \*/

.article {

    font-family: Arial, sans-serif;

}



/\* Specific for most platforms \*/

h1 {

    font-family: "Helvetica Neue", Arial, "Hiragino Sans GB", "WenQuanYi Micro Hei", "Microsoft YaHei", sans-serif;

}

#### \[强制\] font-family 不区分大小写，但在同一个项目中，同样的 Family Name 大小写必须统一。

示例：

/\* good \*/

body {

    font-family: Arial, sans-serif;

}



h1 {

    font-family: Arial, "Microsoft YaHei", sans-serif;

}



/\* bad \*/

body {

    font-family: arial, sans-serif;

}



h1 {

    font-family: Arial, "Microsoft YaHei", sans-serif;

}

