#### \[建议\] 在可以使用缩写的情况下，尽量使用属性缩写。

示例：

/\* good \*/

.post {

    font: 12px/1.5 arial, sans-serif;

}



/\* bad \*/

.post {

    font-family: arial, sans-serif;

    font-size: 12px;

    line-height: 1.5;

}

\[建议\] 使用 border / margin / padding 等缩写时，应注意隐含值对实际数值的影响，确实需要设置多个方向的值时才使用缩写。

解释：

border / margin / padding 等缩写会同时设置多个属性的值，容易覆盖不需要覆盖的设定。如某些方向需要继承其他声明的值，则应该分开设置。

示例：

/\* centering &lt;article class="page"&gt; horizontally and highlight featured ones \*/

article {

    margin: 5px;

    border: 1px solid \#999;

}



/\* good \*/

.page {

    margin-right: auto;

    margin-left: auto;

}



.featured {

    border-color: \#69c;

}



/\* bad \*/

.page {

    margin: 5px auto; /\* introducing redundancy \*/

}



.featured {

    border: 1px solid \#69c; /\* introducing redundancy \*/

}

