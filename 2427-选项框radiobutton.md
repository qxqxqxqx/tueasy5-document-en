# 选项框\_RadioButton ![](/assets/radiobutton.png)

---

> ## 编辑模式

用户可以通过下方编辑模式面板实现对多选项框的显示内容和样式的快速编辑。![](/assets/RadioButtonUser.jpg)注：初始化选中内容填写的是与显示内容相对应的标识字段。

> ## 开发模式

### 参数配置列表

```
{
    'type': 'MultiCheckbox',
    'orient': 'vertical',
    'itemGap': '10px',
    'iconGap': '10px',
    'series': [
        {
            'name': '选项一',
            'value': 'caseInfo'
        },
        {
            'name': '选项二',
            'value': 'police'
        },
        {
            'name': '选项三',
            'value': 'monitor'
        }
    ],
    'checkedValues': [
        'police',
        'caseInfo'
    ],
    'itemStyle': {
        'normal': {
            'color': '#999999',
            'fontSize': '20px',
            'backgroundColor': 'none'
        },
        'checked': {
            'color': '#ffa84e',
            'fontSize': '20px'
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
	<td>MultiCheckBox</td>
</tr>
<tr>
	<td>consist | String</td>
	<td>Color of content, can be parameter of css3 'color'</td>
	<td>checkbox、radio</td>
</tr>
<tr>
	<td>orient | String</td>
	<td>Alignment of optional boxes, 'horizontal' means horizontal alignmenr and 'vertical' means vertical alignment</td>
	<td>horizontal、vertical</td>
</tr>
<tr>
	<td>itemGap | String</td>
	<td>Gap between item and another</td>
	<td></td>
</tr>
<tr>
	<td>iconGap | String</td>
	<td>Gap between check box and input field</td>
	<td></td>
</tr>
<tr>
	<td>series | Array[Object]</td>
	<td>Datas</td>
	<td></td>
</tr>
<tr>
	<td>series[0].name | String</td>
	<td>Content of check box, repeatable</td>
	<td></td>
</tr>
<tr>
	<td>series[0].value | Array[Object]</td>
	<td>Uniquely identification of data, unrepeatable</td>
	<td></td>
</tr>
<tr>
	<td>checkedValues | Array[String]</td>
	<td>Default actived items</td>
	<td></td>
</tr>
<tr>
	<td>itemStyle | Object</td>
	<td>Items style, can be 'normal' or 'checked'</td>
	<td></td>
</tr>
<tr>
	<td>itemStyle.normal | Object</td>
	<td>Unselected style of check box</td>
	<td><pre> {
	//Content color, can be parameter of css3 'color'
	'color': '#999999',
	//Font size, can be parameter of css3 'font-size'
	'fontSize': '20px',
	//Background color, can be parameter of css3 'background-color'
	'backgroundColor': 'none'
  }</pre></td>
</tr>
<tr>
	<td>itemStyle.checked | Object</td>
	<td>Selected style of check box</td>
	<td><pre> {
	'color': '#ffa94e',
	'fontSize': '20px'
  }</pre></td>
</tr>
</table>

> 注：
>
> * 选项框尚未绑定数据时，可以对series进行编辑；选项框绑定数据后，series会自动生成相应信息，用户只可以对name值进行修改
> * 用户定义选项框初始化选中状态时可编辑checkedValues，其他情况下chekedValues会根据用户当前操作进行自动修改
>
> * itemStyle.normal、itemStyle.checked中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他选项框样式



