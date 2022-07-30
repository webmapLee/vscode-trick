# 常用快捷键

- 键盘快捷键设置方式

  ctrl + k 加 ctrl + s

- 新建文件 ： 

  1. **打开新建文件窗口 ctrl + win + alt + n**

  2. **新建文本文件 是  ctrl + n**

  3. **选择语言： ctrl + k  M**

     这个的操作方式是先摁 ctrl +k ，再松开手，摁 M键即

- 生成html文档片段

  可以摁 ! 或者 html:5 这两个字符串，vscode 会提示自动生成html模板

- 快速编写html 标签

  - 嵌套元素，多个重复标签编写方式

    main>nav>ul>li * 3>a* * 2   书写完，直接摁 enter 或者 tab键即可

- 关于代码文件

  打开文件目录：ctrl + e

  切换到特定区块： 如：index.html@  ，注意必须精确找到某一个文件

  切换到指定行： 如：:10 ，跳转到第10行

  跳转到最后一行： fn + 右键

  跳转一个单词：ctrl + 右键

  选取多个重复的单词： 先选中一个单词，然后摁 ctrl + d

  代码上下位移：alt + 上下键

  录屏快捷键：ctrl + alt + r

  变量全局重命名：F2

# 常用技巧

#### 模板字符``中支持自动生成html标签

1. ctrl + , 打开设置，切换为json 模式

2. 添加如下设置

   ```json
   "emmet.includeLanguages": {
       "javascript":"javascriptreact",
       "vue-html":"html",
       "plaintext":"jade"
     },
   ```

   示例中主要是JavaScript 这一项支持自动生成dev标签的

#### 滑鼠

将鼠标光标设置的大点，防止找不到鼠标

#### 赋值一行

在一行的最末尾，摁 ctrl + c    ctrl + v就可以直接复制粘贴这一整行

#### 添加代码片段

打开vscode 设置

示例配置如下：

```json
"query selector":{
    "prefix":"selector",
    "body":[
        "var ${2} = document.querySlector('${1}')"
    ],
    "description":"创建一个query selector"
}
```

然后在代码编辑器中，直接摁 selector ，就会提示你的代码片段，同时摁 tab件就可以切换上面 ${1}  ${2}的位置

同时也可以使用工具VS  Code Snippet Generator

#### 提取一个函数

1. 选取代码块，右键
2. 选择重构，可以把所选的代码放到全局或者当前代码块中的一个函数中

# 工具

#### 文字拼错检查工具

Code Spell Checker

#### 缩排彩虹

indent-rainbow

#### 大括号定位工具

Bracket Pair Colorizer

注意：由于vscode 自身已经支持该功能，所以该工具已经启用

在vscode设置中搜索 @id:editor.bracketPairColorization.enabled @id:editor.guides.bracketPairs  这个进行设置

