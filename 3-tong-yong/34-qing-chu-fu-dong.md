#### \[建议\] 当元素需要撑起高度以包含内部的浮动元素时，通过对伪类设置 clear 或触发 BFC 的方式进

#### 行 clearfix。尽量不使用增加空标签的方式。

解释：

触发 BFC 的方式很多，常见的有：

•	float 非 none

•	position 非 static

•	overflow 非 visible

如希望使用更小副作用的清除浮动方法，参见 A new micro clearfix hack 一文。

另需注意，对已经触发 BFC 的元素不需要再进行 clearfix。

