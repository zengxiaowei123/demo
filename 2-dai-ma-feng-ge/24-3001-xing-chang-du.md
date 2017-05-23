#### **\[强制\]** 每行不得超过 120 个字符，除非单行不可分割。

解释：

常见不可分割的场景为URL超长。

\[建议\] 对于超长的样式，在样式值的 空格 处或 , 后换行，建议按逻辑分组。

示例：

/\* 不同属性值按逻辑分组 \*/

background:

    transparent url\(aVeryVeryVeryLongUrlIsPlacedHere\)

    no-repeat 0 0;



/\* 可重复多次的属性，每次重复一行 \*/

background-image:

    url\(aVeryVeryVeryLongUrlIsPlacedHere\)

    url\(anotherVeryVeryVeryLongUrlIsPlacedHere\);



/\* 类似函数的属性值可以根据函数调用的缩进进行 \*/

background-image: -webkit-gradient\(

    linear,

    left bottom,

    left top,

    color-stop\(0.04, rgb\(88,94,124\)\),

    color-stop\(0.52, rgb\(115,123,162\)\)

\);



