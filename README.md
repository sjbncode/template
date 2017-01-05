# template

http://sike.io/css0to1/taking-the-first-step/

http://sike.io/css0to1/more-content-and-form/

browser-sync start --server --port 4000 --files index.html --files css/main.css
`````````````````
具体的属性排序可以按照以下的规则：

定位属性: position, float, z-index, clear
盒模型相关属性: padding, margin, display, width, height, border
字体相关
CSS2 视觉相关属性 (background)
CSS3 属性 (border-radius, box-shadow)

``````````
块级元素 -
p, div, h1, h2, table, ol 等等
行元素 - 在文字流里面显示，浏览器不会添加断行。默认宽度刚好适应内容。
span, img, a, button, input 等等
我们来看看浏览器怎么渲染这两种不同类型的元素：
灰色背景是块级元素。浏览器会在块级元素前后增加断行。这些元素的默认宽度会填满父容器。
红色背景是行元素，他们的宽度刚好适应内容，而且不会造成断行。

居中 方法1:
display: block; 把行元素变成块元素
margin: 0 auto; 居中块元素
      元素一定要有 width 属性

方法2:
text-align: center; 通过容器来居中行元素

```````````
display:inline   | display:inline-block
inline 元素只能设置其左右内边距和外边距，而不能设置其高度和上下内外边距。和垂直高度有关的 padding, margin, height 都无效。
这时可以使用 display: inline-block。inline-block 元素可以简单理解为对外表现为行元素，而对内表现为块元素。
```````````


border-box 的特性是 padding 和 border 算在你指定的宽度里面，所以宽度你说多少就是多少。下面这张图对比两个宽度同样是 '200px' 

html {
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: inherit;
}
box-sizing: border-box 设定 html 为 border-box
box-sizing: inherit 其他元素基础父元素的 box-sizing 属性

`````````````````