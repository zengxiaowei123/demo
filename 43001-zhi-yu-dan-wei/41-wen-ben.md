#### \[强制\] 文本内容必须用双引号包围。

解释：

文本类型的内容可能在选择器、属性值等内容中。

示例：

/\* good \*/

html\[lang\|="zh"\] q:before {

    font-family: "Microsoft YaHei", sans-serif;

    content: "“";

}



html\[lang\|="zh"\] q:after {

    font-family: "Microsoft YaHei", sans-serif;

    content: "”";

}



/\* bad \*/

html\[lang\|=zh\] q:before {

    font-family: 'Microsoft YaHei', sans-serif;

    content: '“';

}



html\[lang\|=zh\] q:after {

    font-family: "Microsoft YaHei", sans-serif;

    content: "”";

}

