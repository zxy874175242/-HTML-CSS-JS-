# 一些HTML&CSS&JS的相关练习

## ToDoList

> 设计一个TODO List，页面结构如下图所示，要求：
>
> 1. 使用HTML与CSS完成界面开发
> 2. 实现添加功能：输入框中可输入任意字符，按回车后将输入字符串添加到下方列表的最后，并清空输入框
> 3. 实现删除功能：点击列表项后面的“X”号，可以删除该项
> 4. 实现模糊匹配：在输入框中输入字符后，将当前输入字符串与已添加的列表项进行模糊匹配，将匹配到的结果显示在输入框下方。如匹配不到任何列表项，列表显示空

![image-20200807201357884](C:\Users\ZXY\AppData\Roaming\Typora\typora-user-images\image-20200807201357884.png)

- 正则匹配

  ```javascript
  var keyy = new RegExp('要匹配的字符串','gm')
  // 替换颜色
  // 要用innerHTML，不能用innerText,text会把标签直接当成string显示出来
  var newToDo = e.replace(keyy,'<font color=red>$&</font>')
  test.innerHTML = e
  ```

- 检测回车

  绑定``onkeyup`事件,`event.keyCode == 13`

## Canvas画板

