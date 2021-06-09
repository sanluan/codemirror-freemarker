# CodeMirror-FreeMarker mode

## 简介

更新：

freemarker兼容到2.3.31

codemirror兼容到5.52.0

CodeMirror是一款JS编写的在线代码编辑器,本项目是为CodeMirror编写的FreeMarker语法插件

希望对CodeMirror比较熟悉的用户参与到该插件的长期开发中

很遗憾CodeMirror官方已经放弃了freemarker，因此本插件只能作为额外的插件存在
```
    <link rel="stylesheet" type="text/css" href="./lib/codemirror.css" />
    <script src="./lib/codemirror.js"></script>
    <script src="./mode/xml/xml.js"></script>
    <script src="./mode/javascript/javascript.js"></script>
    <script src="./mode/css/css.js"></script>
    <script src="./mode/htmlmixed/htmlmixed.js"></script>
    <script src="./mode/freemarker/freemarker.js"></script>
    <script src="./mode/freemarkermixed/freemarkermixed.js"></script>
    <textarea id="code" name="template">&lt;#assign data={&quot;aa&quot;: .now ,&quot;cc&quot;:&quot;dd&quot;}/&gt;${data.aa!}</textarea>
    <script>
    var editor = CodeMirror.fromTextArea(document.getElementById("code"), {
				mode: "freemarkermixed",
				lineNumbers: true
			});
    </script>
```
更多示例
freemarker语法高亮：mode/freemarker/index.html
freemarker html混合语法高亮：mode/freemarkermixed/index.html

授权:MIT