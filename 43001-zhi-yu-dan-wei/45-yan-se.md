#### \[强制\] RGB颜色值必须使用十六进制记号形式 \#rrggbb。不允许使用 rgb\(\)。

解释：

带有alpha的颜色信息可以使用 rgba\(\)。使用 rgba\(\) 时每个逗号后必须保留一个空格。

示例：

/\* good \*/

.success {

    box-shadow: 0 0 2px rgba\(0, 128, 0, .3\);

    border-color: \#008000;

}



/\* bad \*/

.success {

    box-shadow: 0 0 2px rgba\(0,128,0,.3\);

    border-color: rgb\(0, 128, 0\);

}

#### \[强制\] 颜色值可以缩写时，必须使用缩写形式。

示例：

/\* good \*/

.success {

    background-color: \#aca;

}



/\* bad \*/

.success {

    background-color: \#aaccaa;

}

#### \[强制\] 颜色值不允许使用命名色值。

示例：

/\* good \*/

.success {

    color: \#90ee90;

}



/\* bad \*/

.success {

    color: lightgreen;

}

#### \[建议\] 颜色值中的英文字符采用小写。如不用小写也需要保证同一项目内保持大小写一致。

示例：

/\* good \*/

.success {

    background-color: \#aca;

    color: \#90ee90;

}



/\* good \*/

.success {

    background-color: \#ACA;

    color: \#90EE90;

}



/\* bad \*/

.success {

    background-color: \#ACA;

    color: \#90ee90;

}

