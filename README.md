tHTML学习

# 1. 网页
### 1.1 什么是网页
**网站**是指在因特网根据一定的规则,使用HTML等制作的用于展示特定内容相关的网页集合。
**网页**是网站中的一页,通常是HTML格式的文件,他要通过浏览器来阅读。

网页是构成网站的基本元素,它通常是由图片、链接、文字、声音等元素组成。通常我们看到的网页以 `.htm` 或者 `.html` 结尾

### 1.2 什么是HTML
HTML是一种超文本标记语言,他是用来描述网页的一种语言,不是一种编程语言。


### 1.3 网页的形成
网页是由网页元素组成的,这些元素是利用html标签描述出来,然后通过浏览器解析来显示给用户的。


# 2. 浏览器

### 2.1 常用浏览器
常用的浏览器有IE、火狐、chrome、Safari、Opera、Edge浏览器。

### 2.2 浏览器内核
> 浏览器内核(渲染引擎)：负责读取网页内容、整理讯息、计算网页的显示方式并展示页面。

| 浏览器 | 内核 | 备注| 
| --- | --- | --- |
| IE | Trident | IE、猎豹安全、360极速浏览器、百度浏览器 |
| firefox | Gecko | 火狐浏览器内核 |
| Safari | Webkit | 苹果浏览器内核
| Chrome/Opera | Blink | chrome/ opera浏览器内核。Blink其实是WebKit的分支。|

# 3. Web标准
Web标准是W3C组织和其他标准化组织制定的系列标准的集合。

### 1. 为什么需要Web标准
浏览器不同,显示网页或者排版就有差异。

### 2. Web标准的构成
主要包括 结构(Structure)、表现(Presentation)、行为(Behavior)

| 标准| 说明 |
|  -- | -- |
| 结构 | 结构用于对网页元素进行整理和分类,现阶段主要学的是HTML |
| 表现 | 表现用于设置网页元素的版式、颜色、大小等外观样式,主要指的是CSS |
| 行为 | 行为是指网页模型的定义以及交互的编写,现阶段主要学的是 JavaScript | 


# 3. HTML标签

### 3.1 HTML 标签规范    
1. HTML标签是由尖括号包围的关键词,例如 <html>。
2. HTML标签通常是成对出现的,例如<html>和</html>,我们称之为双标签。标签对中第一个是开始标签,第二个是结束标签。
3. 有些特殊的标签必须是单标签,例如<br />

### 3.2 标签关系
双标签关系可以分为两类: 包含关系 和 并列关系。

1. 包含关系
```html
<head>
    <title></title>
</head>
```

2. 并列关系
```html
<div></div>
<div></div>
```

# 4. HTML基本结构标签

### 4.1 第一个HTML网页
每个网页都会有一个基本的结构标签(也称为骨架标签),页面内容也是在这些基本标签上书写。
HTML页面也称为HTML文档。
```html
<html>
  <head>
    <title>这是网页标签</title>    
  </head>
  <body>
    这是网页内容
  </body>
</html>
```

### 4.2 骨架标签
每个网页都会有一个基本的结构标签(也称为骨架标签),页面内容也是在这些基本标签上书写。
| 标签名 | 定义 | 说明 |
|  --- | --- | --- | 
| `<html></html>` | HTML标签 | 页面中最大的标签,我们称之为根标签 |
| `<head></head>` | 文档头部 | 注意在head标签中我们必须设置的标签是title |
| `<title></title>` | 文档的标题 | 让页面拥有一个属于自己的网页标题 |
| `<body></body>` | 文档的主体 | 元素包含文档的所有内容,页面内容基本都是放到body里面 |

# 5. 标签说明

### 5.1 `<!DOCTYPE>`
`<!DOCTYPE>`  文档类型声明,作用就是告诉浏览器使用哪种HTML版本来显示网页。
`<!DOCTYPE>` 不是一个HTML标签,他就是文档类型声明标签。
```html
<!-- 这句话是告诉浏览器使用html版本来显示网页 -->
<!-- 声明必须位于文档中最前面的位置,位于<html>标签之前 -->
<!DOCTYPE html>
```

### 5.2 `lang`语言种类
用来定义当前文档显示的语言。 en:定义语言为英语、zh-CN:定义语言为中文。 会告诉搜索引擎这是一个什么类型的网站,中文还是英文等。
```html
<html lang="en">
</html>
```

### 5.3 `charset`字符集
字符集是多个字符的集合。以便计算机能够识别和存储各种文字。
在 `<head>`标签内,可以通过 `<meta>` 标签的 `charset`属性来规定HTML文档应该使用哪种字符编码

```html
<meta charset="UTF-8">
```


# 6. HTML常用标签

### 6.1 标签的语义
每个标签都是有各自的作用,可以根据标签的语义,在合适的地方给一个最为合理的标签,可以让页面结构更清晰。


### 6.2 `<h1> - <h6>` 标题标签
为了使网页更具有语义化,我们经常会在页面中用到标题标签。HTML提供了6个等级的网页标题。一般作为标题使用,并且依据重要性递减。
```html
<h1>我是一级标签</h1>
```

特点: 
1. 加了标题的文字会变的加粗,字号也会依次变大。
2. 一个标题独占一行。

### 6.3 `<p></p>` 段落标签
```html
<!-- 可以把HTML文档分割为若干段落 -->
<p>我是一个段落标签</p>
```

特点:
1. 文本在一个段落中会根据浏览器窗口的大小自动换行。
2. 段落和段落之间会有一个空隙

### 6.4 `<br />` 换行标签
```html
<!-- 这是一个换行标签 -->
<br />
```

特点:
1. 是一个单标签
2. 只是换行,并不会增加两行之间的间距。

### 6.5 文本格式化标签
在网页中,有时需要为文字设置 **粗体** 、_斜体_、或者 <u>下划线</u>等效果,这时就需要用到HTML中的文本格式化标签,使文字以特殊的方式显示。

#### 6.5.1 加粗标签
`<strong> </strong>` 加粗标签
```html
<p>我是<strong>加粗</strong>标签</p>
```

`<b> </b>` 加粗标签
```html
<p>我是<b>加粗</b>标签</p>
```

总结:
推荐使用`<strong></strong>`标签,语义更强烈一些。


#### 6.5.2 倾斜标签
`<em></em>`倾斜标签
```html
我是<em>倾斜</em>标签
```

`<i></i>`倾斜标签
```html
我是<i>倾斜</i>标签
```

总结:
推荐使用 `<em></em>` 标签,语义更强烈一些。

### 6.5.3 删除线
`<del></del>`删除线标签
```html
我是<del>删除线</del>标签
```

`<s></s>`删除线标签
```html
我是<s>删除线</s>标签
```

总结:
推荐使用`<del></del>`删除标签,语义更强烈一些。

#### 6.5.4 下划线
`<ins></ins>`下划线标签
```html
我是<ins>下划线</ins>标签
```

`<u></u>`下划线标签
```html
我是<u>下划线</u>标签
```

总结:
推荐使用`<ins></ins>`标签,语义更强烈一些。

### 6.6  `<div></div>` 和 `<span></span>`标签
这两个标签是没有语义的,他们就是一个盒子,用来填装内容的。

```html
<div>我是div标签</div>
```

```html
<span>我是span标签</span>
```

总结:
1. `<div> </div>`标签用来布局,但是现在一行只能放一个此标签。
2. `<span></span>`标签用来布局,一行可以放多个此标签。

### 6.7 `<img />` 标签
在HTML标签中,`<img />`标签用于定义HTML页面中的图像。
```html
<!-- src是img标签的必须属性,它用于指定图像文件的路径和文件名 -->
<img src="图像地址URL" />
```

| 属性 | 属性值 | 说明 |
| --- | --- | --- |
| src | 图片路径 | 必须属性|
| alt | 文本 | 替换文本,图像不能显示时候的文字。|
| title | 文本 | 提示文本,鼠标放到图像上显示的文字。|
| width | 像素 | 设置图像的宽度 |
| height | 像素 | 设置图像的高度 |
| border | 像素 | 设置图像的边框粗细 |

### 6.8 `<a></a>` 超链接标签
在HTML标签中, `<a></a>` 标签用于定义超链接,作用是从一个页面链接到另一个页面。

```html
<a href="跳转目标" target="目标窗口的弹出方式">文本或图像</a>
```

| 属性 | 作用 |
| --- | --- |
| href | 用于指定链接目标的url地址,(必须属性)当为标签应用href属性时,他就具有了超链接的功能 |
| target | 用于指定链接页面的打开方式,其中 `_self` 为默认值, `_blank`为在新窗口中打开方式 |

链接分类:
1. 外部链接
```html
<a href="http://www.baidu.com" target="_blank">百度</a>
```

2. 内部链接
> 网站内部页面之间的相互链接,直接链接内部页面名称即可。
```html
<a href="06-图像标签.html" target="_blank">06-图像标签</a>
```

3. 空链接
> 如果没有确定链接目标的时候,可以使用 #  代替目标

```html
<a href="#">这是一个空链接</a>
```

4. 下载链接
> 下载链接的地址是 文件、压缩包等形式
```html
<a href="下载文件地址">点击下载</a>
```

5. 网页元素超链接
> 在网页中的各种网页元素都可以添加超链接,如文本、图像、表格、音频、视频等。
```html
<a href="http://www.baidu.com"><img src="src/01.png"></a>
```

6. 锚点链接
> 点击链接可以快速定位到页面中的某个位置。
- 在链接文本中的 `href` 属性中,设置属性值为 `#名字名字name` 的形式
```html
<a href="#two">第二季</a>
```
- 找到目标位置标签,在里面添加一个 `id` 属性 = 刚才的名字
```html
<h3 id="two">第二季介绍</h3>
```

### 6.9 HTML中的注释和特殊字符
1. 注释
```html
<!-- 这里是注释 -->
```

2. 特殊字符
```html
讲究 &nbsp; &nbsp; &nbsp; &nbsp; 中间有4个空格
```

| 特殊字符 | 描述 | 字符的代码 |
| --- | --- | --- |
| 空格 | 空格符 | `&nbsp;` |
| < | 小于号 | `&lt;` |
| > | 大于号 | `&gt` |
| & | 和号 | `&amp;` |
| ￥| 人命币 | `&yen;` |
| © | 版权 | `&copy;` |
| ® | 注册商标 | `&reg;` |
| ° | 摄氏度 | `&deg;` |
| ㄨ | 乘号 | `&times;` |
| ÷ | 除号 | `&divide;` |
| ² |  平方2(上标2) | `&sup2;` |
| ³ | 立方3(上标3) | `&sup3;` |


### 6.10 表格标签
表格主要用于显示、展示数据,因为它可以让数据显示的非常的规整,可读性好。特别是后台展示数据的时候,能够熟练运用表格就很重要。一个清爽简约的表格能够把繁杂的数据表现的很有调理。

1. 表格的基本语法
```html
<table>
  <tr>
    <td>单元内的文字</td>
  </tr>
</table>
```

`<table></table>` 是用于定义表格的标签。

`<tr></tr>`标签用于定义表格中的行,必须嵌套在`<table></table>`标签中。

`<td></td>`用于定义表格中的单元格,必须嵌套在`<tr></tr>`标签中。

字母`td`指表格数据(table data),即数据单元格的内容。

2. 表头单元格标签
```html
<table>
  <tr>
    <th>姓名</th>
  </tr>
</table>
```

`<th></th>` 标签标示HTML表格的表头部分(table head)的缩写。一般表头单元格位于表格的第一行或者第一列,表头单元格里面的文本内容加粗居中显示。


3. 表格属性

表格属性一般在实际开发中不常用,后面我们通过CSS来设置。

| 属性名 | 属性值 | 描述 |
| --- | --- | --- |
| align | left、right、center | 规定表格相对周围元素的对齐方式 |
| border | 1 或者 "" | 规定表格单元是否拥有边框,默认为 "", 标示没有边框 |
| cellpadding | 像素值 | 规定单元边沿与其内容之间的空白,默认1像素 |
| cellspacing | 像素值 | 规定单元格之间的空白,默认2像素 |
| width | 像素值或者百分比 | 规定表格的宽度 |
| height | 像素值或者百分比 | 规定表格的高度 |

4. 表格的结构标签

使用场景:因为表格可能很长,为了更好的标示表格的语义,可以将表格分割成表格头部和表格主体两大部分。

在表格标签中,分别用: `<thead></thead>`标签标示表格的头部区域. `<tbody></tbody>`标签来标示表格的主体区域。这样可以更好的分清表格结构。这两个标签都是放在`<table></table>`标签中。

5. 合并单元格

特殊情况下,可以把多个单元格合并为一个单元格。

- 合并单元格的方式：
  
  跨行合并: `rowspan="合并单元格的个数"`
  
  跨列合并: `colspan="合并单元格的个数"`


- 目标单元格

  跨行合并: 最上侧单元格为目标单元格,写合并代码
  
  跨列合并: 最左侧单元格为目标单元格,写合并代码

- 合并单元格三部曲

  首先确定是跨行合并还是跨列合并。

  找到目标单元格,写合并方式 = 合并的单元格数量。 例如: `<td colspan="2></td>`

  删除多余的单元格


  ### 6.11 列表标签

  表格是用来显示数据的,列表就是用来布局的。

  列表最大的特点就是整齐、整洁、有序,它作为布局会更加自由和方便。

  列表可以分为三大类: `无序列表`、`有序列表`、`自定义列表`



1. 无序列表

`<ul></ul>`标签标示HTML页面中项目的无序列表,一般会以项目符号呈现列表项,而列表项使用`<li></li>`标签定义。
  ```html
  <ul>
    <li>列表1</li>
    <li>列表2</li>
    <li>列表3</li>
  </ul>
  ```

  - 无序列表的各个列表之间是没有顺序级别之分,是并列的。

  - `<ul></ul>`中只能嵌套`<li></li>`标签,直接在`<ul></ul>`中输入其他标签或者文字是不允许的。

  - `<li></li>`标签中是可以嵌套任何标签的。

  - 无序列表会带有自己的样式属性,但在实际使用时,我们会使用CSS来设置。


2. 有序列表

  有序了列表即为有序排列的列表,其各个列表项会按照一定的顺序排列定义。

  在HTML标签中,`<ol></ol>`标签用于定义有序列表,列表排序以数字来显示,并且使用`<li></li>`标签来定义列表项。

```html
<ol>
  <li>有序标签1</li>
  <li>有序标签2</li>
  <li>有序标签3</li>
</ol>
```

  - `<ol></ol>`标签中只能嵌套`<li></li>`标签,直接在`<ol></ol>`标签中输入其他标签或者文字是不被允许的。

  - `<li></li>`标签可以容纳所有元素。

  - 有序列表会带有自己的样式属性,但在实际使用时我们会使用CSS来设置覆盖。


3. 自定义列表

自定义列表使用场景: 经常用于对术语或者名词进行解释和描述,定义列表的列表项前没有任何项目和符号。相当于一个大哥带着小弟。

在HTML标签中,`<dl></dl>`标签用于定义描述列表(或定义列表),该标签会与`<dt></dt>`标签(定义项目/名字)和`<dd></dd>`标签(描述每一个项目/名字)一起使用。

```html
<dl>
  <dt>名词1</dt>
  <dd>名词1解释1</dd>
  <dd>名词1解释2</dd>
</dl>
```

- `<dl></dl>`标签中只能包含`<dt></dt>`和`<dd></dd>`

- `<dt></dt>`和`<dd></dd>`个数没有限制,经常是一个`<dt></dt>`对应多个`<dd></dd>`


### 6.12 表单标签

现实生活中的表单:例如去银行办卡,需要先填写一个单子,不通过就直接拒绝下一步。

1. 表单的组成

在HTML中,一个完整的表单通常由 `表单域`、`表单控件(也称为表单元素)`和 `提示信息` 3个部分构成

2. 表单域

`表单域` 就是一个包含表单元素的区域。

在HTML标签中, `<form></form>` 标签用于定义表单域,以实现信息的收集和传递。可以把它范围内的表单元素信息提交给服务器。

```html
<form action="url地址" method="提交方式" name="表单域名称">
  各种表单元素控件
</form>
```

常用属性:

| 属性 | 属性值 | 作用 |
| -- | -- | -- |
| action | url地址 | 用于指定接收并处理表单数据的服务器程序的url地址 |
| method | get/post | 用于设置表单数据的提交方式,其取值为get或post |
| name | 名称 | 用于指定表单的名称,以区分同一个页面中的多个表单域 |

3. `<input />`输入表单元素

```html
<input type="属性值" />
```
| 属性值 | 描述 |
| -- | -- |
| button | 定义可点击按钮(多数情况下,用于通过JavaScript启动脚本) | 
| checkbox | 定义复选框 |
| file | 定义输入字段和"浏览"按钮,供文件上传 |
| hidden | 定义隐藏的输入字段 |
| image | 定义图像形式的提交按钮 |
| password | 定义密码字段。该字段中的字符被掩码 |
| radio | 定义单选按钮 |
| reset | 定义重置按钮。重置按钮会清除表单中的所有数据 |
| submit | 定义提交按钮。提交按钮会把表单数据发送到服务器 |
| text | 定义单行的输入字段,用户可在其中输入文本。默认宽度为20个字符 |


| 属性 | 属性值 | 描述 |
| --- | --- | --- |
| name | 由用户自定义 | 定义input元素的名称 |
| value | 由用户自定义 | 规定input元素的值 |
| checked | checked | 规定此input元素首次加载时应当被选中 |
| maxlength | 正整数 | 规定输入字段中的字符的最大长度 |

- `name` 和 `value` 是每个表单元素都有的属性值,主要给后台人员使用

- `name`表单元素的名字,要求`单选按钮和复选框要有相同的name值`


4. `<label></lable>`标签

此标签为标注标签。`<label></label>`标签用于绑定一个表单元素,当点击`<label></label>`标签内的文本时,浏览器就会自动将焦点(光标)转到或者选择对应的表单元素上,用来增加用户体验。

```html
<label for="sex">男</label>
<input type="radio" name="sex" id="sex" />
```

- `<label?></label>` 标签中的 `for` 属性必须与相关元素的 `id` 属性相同。

5. `<select>`下拉表单元素

```html
<select>
  <option>选项1</option>
  <option>选项2</option>
  <option>选项3</option>
  <option>选项4</option>
</select>
```

- `<select></select>`中至少包含一对`<option></option>`

- 在 `<option></option>`中定义 `selected="selected"`时,当前项即为默认选中项目


6. `<textarea></textarea>`文本域元素

当用户输入内容较多的情况下可以使用此标签

```html
<textarea rows="3" cols="10">
  内容
</textarea>
```

- `cols` = 每行中的字符数, `rows` = 显示的行数。 一般在开发中使用css来改变大小。

