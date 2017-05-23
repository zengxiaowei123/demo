#### **\[强制\]** 当一个 rule 包含多个 selector 时，每个选择器声明必须独占一行。

示例：

/\* good \*/

.post,

.page,

.comment {

    line-height: 1.5;

}



/\* bad \*/

.post, .page, .comment {

    line-height: 1.5;

}

#### \[强制\] &gt;、+、~ 选择器的两边各保留一个空格。

示例：

/\* good \*/

main &gt; nav {

    padding: 10px;

}



label + input {

    margin-left: 5px;

}



input:checked ~ button {

    background-color: \#69C;

}



/\* bad \*/

main&gt;nav {

    padding: 10px;

}



label+input {

    margin-left: 5px;

}



input:checked~button {

    background-color: \#69C;

}

#### \[强制\] 属性选择器中的值必须用双引号包围。

解释：

不允许使用单引号，不允许不使用引号。

示例：

/\* good \*/

article\[character="juliet"\] {

    voice-family: "Vivien Leigh", victoria, female

}



/\* bad \*/

article\[character='juliet'\] {

    voice-family: "Vivien Leigh", victoria, female

}

