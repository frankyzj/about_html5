#### 验证表单输入 {#验证表单输入}

* 必填项：给 
  &lt;
  input
  &gt;
   或者 
  &lt;
  textarea
  &gt;
   元素添加 required 属性。

##### 关闭验证 {#关闭验证}

* 禁用整个表单的验证功能：在 
  &lt;
  form
  &gt;
   元素中添加 novalidate 属性。
* 也可另外添加一个提交按钮，在其中添加 formnovalidate 属性。

#### 设置验证的样式 {#设置验证的样式}

常用的有 required （必填）和 optional （选填）；valid （有效）和 invalid （无效）；

in-range（在范围内）和 out-of-range（超出范围）：根据控件的 min 和 max 属性判断输入值是否超出范围。

例如为必填元素设置背景颜色：

```
input：required{
    background-color：lightyellow；
}

input:required:invalid {
  background-color: lightyellow;
}

```

#### 使用正则表达式验证内容 {#使用正则表达式验证内容}

使用 pattern 属性将正则表达式应用到 &lt;input&gt; 或 &lt;textarea&gt; 元素。

#### H5 规范提供的 JavaScript 属性来验证 {#h5-规范提供的-javascript-属性来验证}

```
setCustomValidity();


<
label for="comments"
>
When did you first know you wanted to be a
 zookeeper?
<
/label
>
<
textarea id="comments" oninput="validateComments(this)" 
>
<
/textarea
>


function validateComments(input) {
  if (input.value.length 
<
 20) {
    input.setCustomValidity("You need to comment in more detail.");
  }
  else {
    //没有错误。清除任何错误消息
    input.setCustomValidity("");
  }
}
```



