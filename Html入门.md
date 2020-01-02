# Html入门笔记
html是用来描述网页的一种超文本标记语言（**Hyper Text Markup Language**）
H5 是最新的标准，H5 默认的字符编码是 UTF-8

* HTML 是谁发明的
是由Web的发明者 Tim Berners-Lee和同事 Daniel W. Connolly于1990年创立的一种标记语言

* HTML 起手应该写什么
```html
<!DOCTYPE HTML>
<html>

</html>
```
* 常用的表章节的标签有哪些，分别是什么意思（h1~h6、section、article、main、aside 等等）
**h1-h6**：设置标题字体大小
**section**：定义一个章节
**article**：定义文章
**main**：定义文章的主要内容 h5新标签  //只能定义一个，不能是article,  nav, footer, header, aside的子标签
**aside**：定义页面内容之外的内容
**form**：定义表单
**p**：定义段落

* 全局属性有哪些
::class::元素类名; dir元素内容的文本方向; ::id::元素唯一的id; lang元素内容语言; ::style::元素样式; title元素额外信息; tabindex元素的tab键次序; accesskey激活元素的快捷键;
contenteditable元素内容是否可编辑; contextmenu元素上下文菜单; draggable元素是否可拖动; dropzone拖动数据是否复制移动或链接; ::hidden::隐藏元素; spellcheck是否对元素进行拼写检查; translate是否翻译元素内容; date-xx储存私有定制数据;

* 常用的内容标签有哪些，分别是什么意思
a：给文本加链接
strong：加粗强调文本
em：斜体强调文本
code：代码文本
small：文本小号字体
<!—xxxxx—>注释
ul：无序列表
style：定义文档样式
script：定义脚本
textarea：多行文本输入控件
title：页面标题
- - - -
### 兼容手机
加上meta:vp
``` html
<meta name='viewport' content="width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0,user-scalable=no">
```
```css
img {
	max-width: 100%;
}
```