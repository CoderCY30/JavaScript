# JavaScript/DOM
<h3>document.documentElement.scrollTop和document.body.scrollTop的区别。</h3>
这两个都是获取滚动条卷进去的高度，区别在于前者是在有DTD(符合Web标准)的情况下，而后而是没有DTD的情况下使用的。<br/>
为了更好的兼容一般情况下写成：<br/>
document.documentElement.scrollTop || document.body.scrollTop<br/>
DTD是指在HTML页面最上方的<!DOCTYPE HTML>声明。<br/>
<h3>document.clientHeight和document.clientWidth。</h3>
clientHeight和clientWidth：可见区域高/宽(不包含滚动条的宽/高，一般是17px)；<br/>
<h3>offsetHeight和offsetWidth。</h3>
元素本身的高/宽，包含内边距和边框，不包括外边距；<br/>
<h3>offsetTop和offsetLeft</h3>
元素本身距离上方(上层控件)/左方(左方控件)的距离。<br/>
Ex:<br/>
&lt;div class="EX"&gt;<br/>
	    &lt;div&gt;ex1&lt;/div&gt;<br/>
	  	&lt;div>ex2&lt;/div&gt;<br/>
&lt;/div&gt;<br/>
ex1的offsetTop是ex1距EX上边框的距离，因为距其上边最近的是EX层的上边框。ex2同理。

