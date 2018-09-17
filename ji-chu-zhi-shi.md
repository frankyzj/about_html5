# 常用标签、属性及注意事项 {#常用标签、属性及注意事项}

&lt;!DOCTYPE html&gt; ： HTML5 的文档类型声明。保证浏览器以比较一致的方式解析文档。

### 内容和结构标签 {#内容和结构标签}

&lt;head&gt;、&lt;body&gt; ： 使文档看起来更清晰。

&lt;title&gt; : 作为标签名显示

&lt;p&gt;：段落

&lt;img&gt;：图片 alt=""，src=""

&lt;input&gt; ： 接收用户输入的微件，type=""

&lt;iframe&gt; ： 用以实现一些集成任务，比如在网页中包含 YouTube 窗口，广告单元和搜索框等。

&lt;small&gt; ： 表示“附属细则”，如页面底部没人看的法律条款。

### 格式标签 {#格式标签}

&lt;em&gt; ： 强调（需要重读的文本），斜体显示

&lt;i&gt;： 需要用斜体显示的文本

&lt;strong&gt; ： 强调，加粗显示

&lt;b&gt; : 需要用粗体表示的文本

&lt;br/&gt; ：换行

&lt;hr/&gt; ： 水平线，在两个区块间画一条线

&lt;s&gt; ： 删除的文本

&lt;a&gt; ：使内部的文本变成蓝色并带有下划线，图像带有蓝色边框

### HTML5 新增的标签 {#html5-新增的标签}

#### 用于构建页面的元素（语义元素） {#用于构建页面的元素（语义元素）}

* **不包含默认样式，不需要命名，可以直接在 css 中引用和应用样式。**

&lt;article&gt;：能够独立的内容区块

&lt;aside&gt;：附注，与周围文本没有密切关系的内容。可以用来放广告、相关内容链接。

&lt;figcaption&gt;：图题，通常和 &lt;img&gt; 元素一起房子 &lt;figure&gt; 元素内。

&lt;figure&gt;：插图，虽然独立于文本，但是文本会提到它。它应该是浮动在离相关文本较近的位置。

&lt;footer&gt;：放网站版权信息、作品来源、法律限制及支持链接，也可以用于文章中的文脚

&lt;header&gt;：可以包含HTML标题和其他内容。其他内容可以是标志、作者署名或一组指向后面内容的导航链接

&lt;hgroup&gt;：主要目的是把标题和副标题联系到一起

&lt;nav&gt;

&lt;section&gt;

&lt;details&gt;

&lt;summary&gt;

#### 用于识别文本的元素 {#用于识别文本的元素}

&lt;mark&gt;

&lt;time&gt;

&lt;wbr&gt;

#### Web 表单及交互 {#web-表单及交互}

&lt;input&gt;

```
//step 属性会影响到数值框的微调按钮。

<
input id="age" type="number" min="0" max="120" step="0.1 value="160"/
>
```

&lt;datalist&gt;

可以在普通文本框中添加下拉建议列表。将 &lt;input&gt; 元素的 list 属性值设置为 &lt;datalist&gt; 的 id。

&lt;keygen&gt;

&lt;meter&gt;

&lt;progress&gt;

&lt;command&gt;

&lt;menu&gt;

&lt;output&gt;

#### 音频、视频及插件 {#音频、视频及插件}

&lt;audio&gt;

&lt;video&gt;

* 有三个常用的属性 controls，metadata，loop

&lt;source&gt;

&lt;embed&gt; ： 向页面中加入插件。

#### Canvas {#canvas}

&lt;canvas&gt;

#### 不支持语义元素的浏览器的处理 {#不支持语义元素的浏览器的处理}

在 CSS 中加入超级规则：

```
article, aside, figure, figcaption, footer, header, hgroup, nav, section,
summary {
  display: block;
}

```

#### HTML 编辑器 {#html-编辑器}

##### 使用 contentEditable 编辑元素。 {#使用-contenteditable-编辑元素。}

##### 使用 designMode 编辑页面 {#使用-designmode-编辑页面}

* 详见 《HTML5 秘籍》电子书 165 页。



