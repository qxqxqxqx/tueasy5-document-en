# 文本框\_Inputtext ![](/assets/inputtext.png)

---


> ## 编辑模式

输入文本框共有两部分组成，标签部分和文本框部分。用户可以通过下方的用户编辑模式面板实现对输入文本框的标签和输入文本颜色、文本大小、边框样式的快速编辑。![](/assets/InputtextUser.jpg)

> ## 开发模式


### 参数配置列表

```
{
	'type': 'Text',
	'label': {
		'text': '标签',
		'style': {
			'normal': {
				'textAlign': 'center',
				'fontSize': '16',
				'fontFamily': 'Hiragino Sans GB',
				'fontWeight': 400,
				'color': '#CCC'
			}
		}
	},
	'input': {
		'value': '',
		'style': {
			'normal': {
				'color': '#333',
				'fontSize': '15',
				'fontFamily': 'Hiragino Sans GB',
				'textAlign': 'center',
				'background': 'none',
				'borderWidth': 1,
				'borderColor': '#4285F4',
				'borderStyle': 'solid',
				'borderRadius': 1
			},
			'mouse': {
				'color': '#333',
				'fontSize': '16',
				'fontFamily': 'Hiragino Sans GB',
				'textAlign': 'center',
				'background': 'none',
				'borderWidth': 1,
				'borderColor': '#4285F4',
				'borderStyle': 'solid',
				'borderRadius': 1
			},
			'emphasis': {
				'color': '#333',
				'fontSize': '15',
				'fontFamily': 'Hiragino Sans GB',
				'textAlign': 'center',
				'background': 'none',
				'borderWidth': 1,
				'borderColor': '#4285F4',
				'borderStyle': 'solid',
				'borderRadius': 1
			}
		}
	}
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
	<td>Text</td>
</tr>
<tr>
	<td>label | Object</td>
	<td>Label of input field, parmeters are 'text' and 'style'</td>
	<td></td>
</tr>
<tr>
	<td>label.text | String</td>
	<td>Text of label</td>
	<td></td>
</tr>
<tr>
	<td>label.style | Object</td>
	<td>Label style of input field, attribute can only be 'normal'</td>
	<td></td>
</tr>
<tr>
	<td>label.style.normal | Object</td>
	<td>Style of label</td>
	<td><pre> {
	//Text horizontal alignment, can be css3 parameters of 'text-align'
	'textAlign': 'center',
	//Font size, can be css3 parameters of 'font-size'
	'fontSize': '16px',
	//Font family, can be css3 parameters of 'font-family'
	'fontFamily': 'Hiragino Sans GB',
	//Font weight, can be css3 parameters of 'font-weight'
	'fontWeight': 400,
	//Text color, can be css3 parameters of 'color'
	'color': '#CCC'
  }</pre></td>
</tr>
<tr>
	<td>input | Object</td>
	<td>Input field, attribute can be 'value' and 'style'</td>
	<td></td>
</tr>
<tr>
	<td>input.value | String</td>
	<td>Content of input field</td>
	<td></td>
</tr>
<tr>
	<td>input.style | Object</td>
	<td>Label style of input field, attribute can be 'normal', 'mouse' or 'emphasis'</td>
	<td></td>
</tr>
<tr>
	<td>input.style.normal | Object</td>
	<td>Unselected style of input field</td>
	<td><pre> {
	//Text color, can be css3 parameters of 'color'
	'color': '#333',
	//Font size, can be css3 parameters of 'font-size'
	'fontSize': '15px',
	//Font family, can be css3 parameters of 'font-family'
	'fontFamily': 'Hiragino Sans GB',
	//Text horizontal alignment, can be css3 parameters of 'text-align'
	'textAlign': 'center',
	//Background style, can be css3 parameters of 'background'
	'background': 'none',
	//Border width, can be css3 parameters of 'border-width'
	'borderWidth': 1px,
	//Border color, can be css3 parameters of 'border-color'
	'borderColor': '#4285F4',
	//Border style, can be css3 parameters of 'border-style'
	'borderStyle': 'solid',
	//Border radius, can be css3 parameters of 'border-radius'
	'borderRadius': '1px'
  }</pre></td>
</tr>
<tr>
	<td>input.style.mouse | Object</td>
	<td>Hovered style of input field</td>
	<td><pre> {
	'color': '#333',
	'fontSize': '16px',
	'fontFamily': 'Hiragino Sans GB',
	'textAlign': 'center',
	'background': 'none',
	'borderWidth': 1px,
	'borderColor': '#4285F4',
	'borderStyle': 'solid',
	'borderRadius': '1px'
  }</pre></td>
</tr>
<tr>
	<td>input.style.emphasis | Object</td>
	<td>Selected style of input field</td>
	<td><pre> {
	'color': '#333',
	'fontSize': '15px',
	'fontFamily': 'Hiragino Sans GB',
	'textAlign': 'center',
	'background': 'none',
	'borderWidth': 1px,
	'borderColor': '#4285F4',
	'borderStyle': 'solid',
	'borderRadius': '1px'
  }</pre></td>
</tr>
</table>

> 注：
>
> * style.normal、style.mouse、style.emphasis中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他文本框样式



