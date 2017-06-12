# 按钮\_basicButton ![](/assets/basicButton.png)

---

> ## 编辑模式

用户可以通过下方的用户编辑模式面板实现对按钮样式的快速编辑。![](/assets/buttonUser.jpg)

> ## 开发模式

### 参数配置列表

```
{
	'type': 'TheButton',
	'normal': {
		'backgroundColor': '#31b16c',
		'fontSize': '20',
		'borderRadius': 5,
		'borderColor': '#31b16c',
		'borderWidth': 1,
		'borderStyle': 'solid',
		'color': '#fff',
		'lineHeight': '47px',
		'textAlign': 'center',
		'cursor': 'pointer',
		'opacity': 0.6
	},
	'mouse': {
		'backgroundColor': '#31b16c',
		'borderRadius': 5,
		'fontSize': '20',
		'borderColor': '#31b16c',
		'borderWidth': 1,
		'borderStyle': 'solid',
		'color': '#fff',
		'lineHeight': '47px',
		'textAlign': 'center',
		'cursor': 'pointer',
		'opacity': 0.8
	},
	'emphasis': {
		'backgroundColor': '#31b16c',
		'borderRadius': 5,
		'fontSize': '20',
		'lineHeight': '47px',
		'color': '#fff',
		'textAlign': 'center',
		'borderColor': '#31b16c',
		'borderWidth': 1,
		'borderStyle': 'solid',
		'opacity': 0.7
	},
	'selected': false,
	'text': '确 认'
}
```

### 参数字段说明

<table border="1">
<tr>
	<th width="15%">Configuration item</th>
	<th width="30%">Description</th>
	<th>Optional parameters</th>
</tr>
<tr>
	<td>type | String</td>
	<td>Component type, unchangeable</td>
	<td>Button</td>
</tr>
<tr>
	<td>normal | Object</td>
	<td>Unselected style of button</td>
	<td><pre> {
	//Background color, can be parameter of css3 'background-color'
	'backgroundColor': '#31b16c',
	//Font size, can be parameter of css3 'font-size'
	'fontSize': '20px',
	//Border radius, can be parameter of css3 'border radius'
	'borderRadius': '5px'
	//Border color, can be parameter of css3 'border-color'
	'borderColor': '#31b16c',
	//Border width, can be parameter of css3 'border-width'
	'borderWidth': 1px,
	//Border style, can be parameter of css3 'border-style'
	'borderStyle': 'solid',
	//Text color, can be parameter of css3 'color'
	'color': '#fff'
	//Line height, can be parameter of css3 'line-height'
	'lineHeight': '47px',
	//Text horizontal alignment, can be parameter of css3 'text-align'
	'textAlign': 'center',
	//Cursor style, can be parameter of css3 'cursor'
	'cursor': 'pointer',
	//Opacity of button, can be parameter of css3 'opacity'
	'opacity': 0.6
  }</pre></td>
</tr>
<tr>
	<td>mouse | Object</td>
	<td>Hovered style of button</td>
	<td><pre> {
	'backgroundColor': '#31b16c',
	'fontSize': '20px',
	'borderRadius': '5px'
	'borderColor': '#31b16c',
	'borderWidth': 1px,
	'borderStyle': 'solid',
	'color': '#fff'
	'lineHeight': '47px',
	'textAlign': 'center',
	'cursor': 'pointer',
	'opacity': 0.8
  }</pre></td>
</tr>
<tr>
	<td>emphasis | Object</td>
	<td>Selected style of button</td>
	<td><pre> {
	'backgroundColor': '#31b16c',
	'fontSize': '20px',
	'borderRadius': '5px'
	'borderColor': '#31b16c',
	'borderWidth': 1px,
	'borderStyle': 'solid',
	'color': '#fff'
	'lineHeight': '47px',
	'textAlign': 'center',
	'cursor': 'pointer',
	'opacity': 0.7
  }</pre></td>
</tr>
<tr>
	<td>selected | Bool</td>
	<td>Whether or not to be selected</td>
	<td></td>
</tr>
<tr>
	<td>text | String</td>
	<td>Content of button</td>
	<td></td>
</tr>
</table>

> 注：
>
> * normal、mouse、emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他按钮样式



