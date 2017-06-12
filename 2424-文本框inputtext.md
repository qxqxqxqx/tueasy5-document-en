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
	<td>输入文本框的提示标签的样式</td>
	<td><pre> {
	//文本水平对齐方式，支持CSS3中text-align的参数值
	'textAlign': 'center',
	//文本大小，支持CSS3中font-size的参数值
	'fontSize': '16px',
	//文本样式，支持CSS3中font-family的参数值
	'fontFamily': 'Hiragino Sans GB',
	//文本粗细，支持CSS3中font-weight的参数值
	'fontWeight': 400,
	//文本颜色，支持CSS3中颜色的参数值
	'color': '#CCC'
  }</pre></td>
</tr>
<tr>
	<td>input | Object</td>
	<td>输入文本框的输入框，有value和style两个属性</td>
	<td></td>
</tr>
<tr>
	<td>input.value | String</td>
	<td>输入文本框的输入框的文本内容</td>
	<td></td>
</tr>
<tr>
	<td>input.style | Object</td>
	<td>输入文本框的提示标签的样式，有normal、mouse和emphasis三个属性</td>
	<td></td>
</tr>
<tr>
	<td>input.style.normal | Object</td>
	<td>输入文本框的输入框<b>未选中</b>状态的样式</td>
	<td><pre> {
	//文本颜色，支持CSS3中颜色的参数值
	'color': '#333',
	//文本大小，支持CSS3中font-size的参数值
	'fontSize': '15px',
	//文本样式，支持CSS3中font-family的参数值
	'fontFamily': 'Hiragino Sans GB',
	//文本水平对齐方式，支持CSS3中text-align的参数值
	'textAlign': 'center',
	//背景样式，支持CSS3中background的参数值
	'background': 'none',
	//边框宽度，支持CSS3中border-width的参数值
	'borderWidth': 1px,
	//边框颜色，支持CSS3中border-color的参数值
	'borderColor': '#4285F4',
	//边框样式，支持CSS3中border-style的参数值
	'borderStyle': 'solid',
	//边框圆角角度，支持CSS3中border-radius的参数值
	'borderRadius': '1px'
  }</pre></td>
</tr>
<tr>
	<td>input.style.mouse | Object</td>
	<td>输入文本框的输入框<b>鼠标悬浮</b>状态的样式</td>
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
	<td>输入文本框的输入框<b>选中</b>状态的样式</td>
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



