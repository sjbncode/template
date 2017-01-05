# template

http://sike.io/css0to1/taking-the-first-step/

http://sike.io/css0to1/more-content-and-form/

browser-sync start --server --port 4000 --files index.html --files css/main.css

具体的属性排序可以按照以下的规则：

定位属性: position, float, z-index, clear
盒模型相关属性: padding, margin, display, width, height, border
字体相关
CSS2 视觉相关属性 (background)
CSS3 属性 (border-radius, box-shadow)

``````````
display:inline   | display:inline-block
inline 元素只能设置其左右内边距和外边距，而不能设置其高度和上下内外边距。和垂直高度有关的 padding, margin, height 都无效。
这时可以使用 display: inline-block。inline-block 元素可以简单理解为对外表现为行元素，而对内表现为块元素。
```````````