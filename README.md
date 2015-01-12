Tieba Sublime Snippets
=======
Tieba 常用代码片段 for Sublime Text 2/3。安装方式分为1,2，推荐使用第一种，snippet更新会自动更新本地

## 安装1-会自动更新

1. 打开 Package Control（快捷键：`shift + cmd + P`），找到命令`Package Control: Add Repository`并执行；
2. 键入`https://github.com/tbfe/Surf-Sublime`；
3. 再次打开 Package Control（快捷键：`shift + cmd + P`），找到命令`Package Control: Install Package`并执行；如果之前已经安装，则搜素Update Package
4. 找到`Surf-Sublime`回车完成安装。


## 安装2-不会自动更新
1.clone项目，把下面后缀名sublime-snippet的文件放在`{SublimeTextData}/Package/User`

## 使用
下面是可用命令列表，输入会有自动提示

### 下面tbjs的提示
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

### 下面是tb php 描述
|命令|描述|
|----|----|
tblayout|layout invoke
tbwidget|load widget
tbgetPageData|getPageData
tbscriptStart|use js in php
tbfunnote|the same to tbjs tbfunnote

### 下面是tb ng 描述
|命令|描述|
|----|----|
tbng-button|button for ngmis
tbng-form-group|form group fowr ngmis
tbng-input-error|warning tips for ngmis
tbng-textarea|simple textarea for ngmis
tbng-input-text|simple text input for ngmis
tbng-input-image|image input for ngmis
tbng-modal|modal template for ngmis

## 贡献
### 新增 snippet
1. Tools > New Snippet，代码片段示例如下，后缀名为`sublime-snippet`。另外请注意，`*.html`文件作为标记语言的scope值应为`text.html`(参考:[Syntax Definitions](http://docs.sublimetext.info/en/latest/extensibility/syntaxdefs.html?highlight=scope))

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
2. 执行上面安装，该文档默认会保存至`{SublimeTextData}/Package/Tieba-Sublime-Snippets`目录下，可在本地测试。
3. 将该文件复制到本项目目录，更新 Readme 中的「命令列表」部分。
4. 提交。

## 参考文档
- http://docs.sublimetext.info/en/latest/extensibility/snippets.html
- http://www.cnblogs.com/yili16438/p/3734343.html
- http://mandymadethis.com/sharing-sublime-text-snippets/
