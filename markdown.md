# sublime-Markdown setting

| 插件 | 功能 |
|---- |---- |
|**MarkdownEditing**|提高Sublime中Markdown编辑特性|
|**MarkdownPreview**|Markdown转HTML，在浏览器中预览|
|**LiveReload**|提供md/html等文档的实时刷新预览|


# 0. 插件安装
1. 组合键<font color=#FF0000>`Ctrl+Shift+P`</font>调出命令面板  
2. 输入<font color=#FF0000>`Package Control: Install Package`</font>，回车  
3. 在搜索框中输入要安装的包名  

# 1. Markdown Preview
## 安装 & 配置
组合键<font color=#FF0000>`Ctrl+Shift+P`</font>调出命令面板, 找到并选中<font color=#FF0000>Markdown Preview</font>  
自定义快捷键：打开<font color=#FF0000>Preferences -> Key Bindings</font>添加一行代码：
``` 
{ "keys": ["alt+m"], "command": "markdown_preview", "args": {"target": "browser", "parser":"markdown"}  }
```
打开自动重载：打开其配置文件 <font color=#FF0000>Preferences -> Package Settings -> Markdown Preview -> Settings</font>，检查左侧enable_autoreload条目是否为true，若不是,右侧栏加一条：
```
{
    "enable_autoreload": true
}
```
#2. Markdown LiveReload
## 安装并配置LiveReload
<font color=FF0000>`Ctrl+shift+p`</font>, 输入<font color=#FF0000>LiveReload: Enable/disable plug-in</font>, 选择<font color=#FF0000>Simple Reload</font>或<font color=#FF0000>Simple Reload with delay (400ms)</font>