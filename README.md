Tieba Sublime Snippets
=======
Tieba 常用代码片段 for Sublime Text 2/3。

##安装

1. 打开 Package Control（快捷键：`shift + cmd + P`），找到命令`Package Control: Add Repository`并执行；
2. 键入`https://github.com/tbfe/Tieba-Sublime-Snippets`；
3. 再次打开 Package Control（快捷键：`shift + cmd + P`），找到命令`Package Control: Install Package`并执行；
4. 找到`Tieba-Sublime-Snippets`回车完成安装。

##使用
下面是可用命令列表，输入会有自动提示

|命令|描述|
|----|----|
tbwidget|gennate a widget js
tbscriptStart|use script
tbdialog|dialog
dialog.onaccept|dialog
dialog.oncancel|dialog
tbtrack|dialog
tbjsload|JsLoadManager
tbcookie|cookie
tbdateFormat|dateFormate
tbfilenote|file note
tbfunnote|fun note
tbrequireInstance|this.requireInstance
tbalert|alert
tbdisableInput|disableInput

##贡献
###新增 snippet
1. Toos > new snippet ，代码片实例如下，后缀名为`sublime-snippet`

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
2. 该文档默认会保存至`{SublimeTextData}/Package/User`目录下，可在本地测试。
3. 将该文件复制到本项目目录，更新 Readme 中的「命令列表」部分。
4. 提交。

## 参考文档
http://docs.sublimetext.info/en/latest/extensibility/snippets.html
http://www.cnblogs.com/yili16438/p/3734343.html
http://mandymadethis.com/sharing-sublime-text-snippets/
