##how to install

1. shift + cmd + P Package Control: Add Repository
2. Add the link to your repo: https://github.com/tbfe/Tieba-Sublime-Snippets
3. Now install the snippets: shift + cmd + P ,again
4. Install Package
5. Search for the repo name:Tieba-Sublime-Snippets
Start using your new snippet collection!

## 自动提示,输入tb
```
tbwidget == gennate a widget js
tbscriptStart ==use script
tbdialog   ==dialog
dialog.onaccept ==dialog
dialog.oncancel ==dialog
tbtrack   ==dialog
tbjsload  == JsLoadManager
tbcookie == cookie
tbdateFormat  ==dateFormate
tbfilenote ==file note
tbfunnote == fun note
tbrequireInstance == this.requireInstance
tbalert == alert
tbdisableInput  ==  disableInput
```

##如何新建一个snippet ，toos new snippet 

```
<!-- Optional:代码片段 ，对某些特殊字符转义,$1,$2代表tab跳转到的位置-->
<snippet>
	<content><![CDATA[
\$.stats.track(${1:'locate'}, ${2:'task'}, ${3:'page'}, ${4:extra})
});
]]></content>
	<!-- Optional:快捷触发  Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>tbjsload</tabTrigger>
	<!-- Optional:作用域 Set a scope to limit where the snippet will trigger -->
	<scope>source.js</scope>
		<!-- Optional:描述 -->
	<description>$.JsLoadManager</description>
</snippet>

```
##参考文档
http://docs.sublimetext.info/en/latest/extensibility/snippets.html
http://www.cnblogs.com/yili16438/p/3734343.html
http://mandymadethis.com/sharing-sublime-text-snippets/
