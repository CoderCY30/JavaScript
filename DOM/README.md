# JavaScript/DOM
<h3>document.documentElement.scrollTop和document.body.scrollTop的区别。</h3>
这两个都是获取滚动条卷进去的高度，区别在于前者是在有DTD(符合Web标准)的情况下，而后而是没有DTD的情况下使用的。<br/>
为了更好的兼容一般情况下写成：<br/>
document.documentElement.scrollTop || document.body.scrollTop<br/>
DTD是指在HTML页面最上方的<!DOCTYPE HTML>声明。
