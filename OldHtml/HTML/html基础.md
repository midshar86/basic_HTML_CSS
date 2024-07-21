# HTML常用标签

## 1.&lt;b&gt;标签与&lt;strong&gt;标签

用来实现文本的 **强调效果**, &lt;strong&gt; 标签语义性更强.

## 2.&lt;i&gt;标签与&lt;em&gt;标签

用来实现文本的 ***倾斜效果*** ,&lt;em&gt; 标签语义性更强.

==Attention1:==
> 当应当作为双标签的标签省略了结束标签, 而是两个开始标签, html 文档会将后面的所有内容作为标签中的内容, 因为开始标签会向后寻找结束标签, 没有结束标签, 搜索会一直持续下去.
> 例如下面的 html 代码中的&lt;b&gt;标签会覆盖之后的所有文本
>
`<div>This is <b>a text paragraph<b> using to test the html sign.</b>`
***
==Attention2:==
> 标签之间可以存在嵌套行为, 但是嵌套的标签不能够尽心交叉嵌套, 这是不符合语法规范的.
> 例如下面的代码是不合法的
`<div>I have a pen, and you have an apple, but <i>we <b>don't</i> like</b> it.</div>`

## 3.&lt;u&gt;标签

用来为文本增加<u>**下划线效果**</u>.

## 4.&lt;s&gt;标签与&lt;del&gt;标签

用来为文本添加<b>~~删除线效果~~</b>, &lt;del&gt; 标签语义化更强.

## 5.&lt;sub&gt;标签与&lt;sup&gt;标签

用来为文本增加下标与上标, 使用 &lt;sub&gt; 标签增加~下标~, 使用 &lt;sup&gt; 增加^上标^.

## 6.&lt;br/&gt;标签

用来为文本执行强制换行.

## 7.&lt;p&gt;标签

用来形成自然段的文本.

==Tips:在 VScode 中, 可以使用 Lorem 提示词创建随机文本.==

## 8.&lt;hr/&gt;标签

用来分隔文本, 显示为一条贯穿浏览器窗口的横线.
> &lt;hr/&gt; 标签的一些属性
>
> + noshade 属性, 控制阴影
> + color 属性, 设置水平线的颜色
> + size 属性, 设置水平线的粗细
> + width 属性, 设置水平线的长度
> + align 属性,设置水平线的对其方式 (left/center/right)

## 9.&lt;h1&gt;~&lt;h6&gt;标题标签

用来生成文本的标题.

==Tips:关于使用 VScode 创建标签的一些快捷键==

> 1. 标签名*num ==> 快速创建 num 个标签
> 2. 标签名 {text}*num ==> 快速创建 num 个带有 test 文本的标签
> 3. h${text}*num ==> 快速创建 &lt;h1&gt;~&lt;h num&gt; 并且带有 text 文本的一系列标题

## 10.&lt;ol&gt;标签、&lt;ul&gt;标签与&lt;li&gt;标签

用来创建列表及列表项目.

&lt;ol&gt; 标签用来创建有序列表, &lt;ul&gt; 标签用来创建无序列表, &lt;li&gt; 标签用来创建列表项.
> 在 &lt;ol&gt; 标签中, 可以设置 type 属性为 1、a、A、I、i.
> 在 &lt;ul&gt; 标签中, 可以设置 type 属性为 disc、circle、square.

==Tips:关于使用 VScode 创建标签的一些快捷键==

> 1. 父标签名>子标签名 ==> 快速创建父子关系的标签
> 2. 父标签名>子标签名*num ==> 快速创建一个含有 num 个子标签的父标签
> 3. 父标签名>子标签名{text}*num ==> 快速创建一个含有 num 个内容是 text 的父标签

## 11.&lt;dl&gt;标签、&lt;dt&gt;标签与&lt;dd&gt;标签

用来生成自定义列表, 通常用于图文混排.

## 12.&lt;img/&gt;标签

用来在 html 中插入图片.
> &lt;img/&gt; 元素的一些属性:
>
> + src 属性用来指定引用的图片源
> + alt 属性用来指定在浏览器中加载失败时显示信息
> + title 属性用来指定当鼠标悬停在图片上时显示的信息.

## 13.&lt;a&gt;标签

用来生成跳转连接, 可以跳转至绝对路径与相对路径.
> &lt;a&gt; 元素的一些属性:
>
> + href 属性用来设置跳转链接
> + target 属性用来设置目标链接的打开位置, 可选值有 _self、_blank

&lt;a&gt; 标签可以利用 href 属性与中的锚点结合页面中其余标签的 id 属性值进行跳转.

```html
<a href="#jumpHere">click to jump another link.</a>
<div>
    <p id="jumpHere">You will get here.</p>
</div>
```

## 14.&lt;div&gt;标签与&lt;span&gt;标签

用来划分页面的布局, 两个标签都没有实际的意义.
&lt;div&gt; 标签用来划分页面的块, 展示整体的效果; &lt;span&gt; 标签用来修饰局部文本.

## 15.&lt;font&gt;标签

用来修饰文本.
> &lt;font&gt;元素的一些属性:
>
> + size 属性用来设置文本大小
> + face 属性用来设置字体格式
> + color 属性用来设置文本颜色

## 16.&lt;form&gt;标签

用来创建表单.
> &lt;form&gt; 元素的一些属性:
>
> + action 属性, 用来指定数据提交的服务器地址
> + method 属性, 用来指定数据以 get 或者 post 方式提交
> + target 属性, 用来指定提交数据后新打开的窗口在什么位置打开

## 17.&lt;input&gt;标签

用来在表单中形成文本框、选项及按钮. 在该标签中, 有 type属性、name属性、placeholder属性、value属性等.

该元素的样式及作用与 type 属性相关联. 不同的取值对应着不同的功能.
> &lt;input&gt;元素 type 属性的一些取值:
>
> + text 取值, 用来作为普通的输入框
> + button 取值, 用来作为普通的按钮
> + password 取值, 用来作为密码框,
> + submit 取值, 用来作为提交按钮
> + reset 取值, 用来重置表单的输入内容
> + radio 取值, 用来作为单选按钮
> + checkbox 取值, 用来作为复选框
> + color 取值, 添加取色板输入控件
> + number 取值, 文本框仅支持数字输入
> + date 取值, 添加日期输入控件
> + email 取值, 用来支持电子邮件格式输入
> + range 取值, 添加范围选择控件
> + file 取值, 添加上载文件控件
> + tel 取值, 用来支持在文本框中输入电话格式
> + url 取值, 用来支持在文本框中输入URL格式
> + 等等

value 属性是指用户在输入框中输入的文本值. name 属性是指当该输入框中的内容被提交给服务器后, value 属性值会与 name 属性值作为名值对的形式被绑定.

## 18.字符实体

在书写 html 文档时, 要想在页面中显示一些特殊符号, 往往需要用到字符实体. 字符实体的格式是使用&符号与一个英文缩写或者数字编码, 最后是一个分号.

> 下面是一些常用的字符实体:
>
> + "<" : "&amp;lt;"
> + ">" : "&amp;gt;"
> + "&" : "&amp;amp;"
> + ' " ' : "&amp;quot"
> + "™" : "&amp;trade"
> + "®" : "&amp;reg"
> + 半角空格 : "&amp;nbsp;"
> + 全角空格 : "&amp;emsp;"
> + "©" : "&amp;copy;"
