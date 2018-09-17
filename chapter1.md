# 基础知识 {#基础知识}

#### 字符编码 {#字符编码}

&lt;meta charset="utf-8" /&gt; ： 置于文档类型声明之后，或者 &lt;head&gt; 标签首行，说明页面的编码字符类型，否则，火狐无法识别汉字。

#### 页面语言 {#页面语言}

通过在任何元素上使用 lang 属性，指明其使用的自然语言。

为整个页面添加语言说明：

```
<
html lang="en"
>
```

#### 添加样式表（链接到相应的css） {#添加样式表（链接到相应的css）}

在 &lt;head&gt; 中添加 &lt;link&gt; 元素。例如：

```
<
link href="styles.css" rel="stylesheet"
>
```

#### 添加 JavaScript {#添加-javascript}

```
<
script src="scripts.js"
>
<
/script
>
```

必须使用完整的标签命名 &lt;script&gt;&lt;/script&gt;，否则页面不会加载脚本。

如果要在 IE 中测试包含 js 的页面，要在 &lt;head&gt; 中字符编码声明下加入如下注释：

```
<
!-- saved from url=(0014)about:internet --
>
```

告知 IE 将页面视为从远程网站上下载的。否则会弹出安全警告。

#### 块级元素和行级元素 {#块级元素和行级元素}

#### 其他 {#其他}

* 浏览器会忽略它不支持的标签，只显示它认识的标签。



