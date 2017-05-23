#### \[建议\] 同一 rule set 下的属性在书写时，应按功能进行分组，并以 Formatting Model（布局方式、

#### 位置） &gt; Box Model（尺寸） &gt; Typographic（文本相关） &gt; Visual（视觉效果） 的顺序书写，以提

#### 高代码的可读性。

解释：

•	Formatting Model 相关属性包括：position / top / right / bottom / left / float / display / overflow 等

•	Box Model 相关属性包括：border / margin / padding / width / height 等

•	Typographic 相关属性包括：font / line-height / text-align / word-wrap 等

•	Visual 相关属性包括：background / color / transition / list-style 等

另外，如果包含 content 属性，应放在最前面。

示例：

.sidebar {

    /\* formatting model: positioning schemes / offsets / z-indexes / display / ...  \*/

    position: absolute;

    top: 50px;

    left: 0;

    overflow-x: hidden;



    /\* box model: sizes / margins / paddings / borders / ...  \*/

    width: 200px;

    padding: 5px;

    border: 1px solid \#ddd;



    /\* typographic: font / aligns / text styles / ... \*/

    font-size: 14px;

    line-height: 20px;



    /\* visual: colors / shadows / gradients / ... \*/

    background: \#f5f5f5;

    color: \#333;

    -webkit-transition: color 1s;

       -moz-transition: color 1s;

            transition: color 1s;

}

