#### \[强制\] 必须同时给出水平和垂直方向的位置。

解释：

2D 位置初始值为 0% 0%，但在只有一个方向的值时，另一个方向的值会被解析为 center。为避免理解上的困扰，应同时给出两个方向的值。background-position属性值的定义

示例：

/\* good \*/

body {

    background-position: center top; /\* 50% 0% \*/

}



/\* bad \*/

body {

    background-position: top; /\* 50% 0% \*/

}

