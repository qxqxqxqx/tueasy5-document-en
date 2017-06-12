# 导航\_linesNav ![](/assets/linesNav.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'currentSelect': 0,
    'automatic': {
        'start': false,
        'interval': 2000
    },
    'maxNumInOneLine': 100,
    'animation': {
        'showAnimation': true,
        'animationType': 'withLines',
        'animationDelay': 1000
    },
    'orient': 'horizontal',
    'series': [
        {
            'type': 'lattice',
            'data': [
                {
                    'key': 'create',
                    'name': '创业'
                },
                {
                    'key': 'map',
                    'name': '地图'
                },
                {
                    'key': 'police',
                    'name': '交警'
                },
                {
                    'key': 'managerPolice',
                    'name': '城管'
                },
                {
                    'key': 'fire',
                    'name': '消防'
                }
            ],
            'textStyle': {
                'normal': {
                    'fontSize': '18px',
                    'color': '#ffa84e'
                },
                'emphasis': {
                    'fontSize': '18px',
                    'color': '#ffa84e'
                }
            },
            'backgroundPathStyle': {
                'normal': {
                    'color': '#ffe3c6',
                    'stroke': '#ffe3c6',
                    'opacity': 0
                },
                'emphasis': {
                    'stroke': '#ffe3c6',
                    'opacity': 1
                }
            },
            'bothSidesStyle': {
                'normal': {
                    'borderColor': '#ffd3a6'
                },
                'emphasis': {
                    'borderColor': '#f6eb3f'
                }
            }
        }
    ],
    'itemGap': '24'
}
```

### 参数字段说明

<table border="1">
<tr>
<th width="15%">Configuration item</th>
<th width="50%">Description</th>
<th>Optional parameters</th>
</tr>
<tr>
<td>currentSelect | Number</td>
<td>Default active tab</td>
<td></td>
</tr>
<tr>
<td>automatic | Object</td>
<td>Automatically switch tabs, parameter can be 'start' or 'interval'</td>
<td></td>
</tr>
<tr>
<td>automatic.start | Bool</td>
<td>Whether or not to switch tabs automatically</td>
<td></td>
</tr>
<tr>
<td>automatic.interval | Number</td>
<td>Time interval to switch tabs in milliseconds.Works only when 'start' is true</td>
<td></td>
</tr>
<tr>
<td>maxNumInOneLine | Number</td>
<td>Maximum number of tabs in one line</td>
<td></td>
</tr>
<tr>
<td>animation | Object</td>
<td>Animation of a hovered tab, parameter can be 'showAnimation', 'animationType' or 'animationDelay'</td>
<td></td>
</tr>
<tr>
<td>animation.showAnimation | Bool</td>
<td>Whether or not to show animation</td>
<td></td>
</tr>
<tr>
<td>animation.animationType | String</td>
<td>Animation type</td>
<td>lattice</td>
</tr>
<tr>
<td>animation.animationDelay | Number</td>
<td>Animation delay time, that is time interval after a tab is hovered with the animation start in milliseconds</td>
<td></td>
</tr>
<tr>
<td>orient | String</td>
<td>Layout direction of tabs</td>
<td>horizontal</td>
</tr>
<tr>
<td>series | Array[Object]</td>
<td>Data and styles</td>
<td></td>
</tr>
<tr>
<td>series[0].type | String</td>
<td>Component type, unchangeable</td>
<td>withLines</td>
</tr>
<tr>
<td>series[0].data | Array[Object]</td>
<td>Data of tabs</td>
<td></td>
</tr>
<tr>
<td>series[0].data[0].key | String</td>
<td>Uniquely identification of data, not repeatable</td>
<td></td>
</tr>
<tr>
<td>series[0].data[0].name | String</td>
<td>Text of tab</td>
<td></td>
</tr>
<tr>
<td>series[0].textStyle | Object</td>
<td>Text style of tab, parameter can be 'normal' or 'emphasis'</td>
<td></td>
</tr>
<tr>
<td>series[0].textStyle.normal | Object</td>
<td>Text style of normal tab</td>
<td><pre> {
//all css3 parameters'font-size'
'fontSize': '18px',
//all css3 parameters of 'color'
'color': '#ffa84e'
}</pre></td>
</tr>
<tr>
<td>series[0].textStyle.emphasis | Object</td>
<td>Text style of emphasis tab</td>
<td><pre> {
'fontSize': '18px',
'color': '#ffa84e'
}</pre></td>
</tr>
<tr>
<td>series[0].backgroundPathStyle | Object</td>
<td>Background slash of tabs, parameter can be 'normal' or 'emphasis'</td>
<td></td>
</tr>
<tr>
<td>series[0].backgroundPathStyle.normal | Object</td>
<td>Background slash style of normal tab</td>
<td><pre> {
//all css3 parameters of 'color'
'stroke': '#ffe3c6',
//Opacity of backgorund slash, parameter can be number from 0.0 to 1.0
'opacity': 0
}</pre></td>
</tr>
<tr>
<td>series[0].backgroundPathStyle.emphasis | Object</td>
<td>Background slash style of emphasis tab</td>
<td><pre> {
'stroke': '#ffe3c6',
'opacity': 1
}</pre></td>
</tr>
<tr>
<td>series[0].bothSidesStyle | Object</td>
<td>Left and right border style of tabs, parameter can be 'normal' or 'emphasis'</td>
<td></td>
</tr>
<tr>
<td>series[0].bothSidesStyle.normal | Object</td>
<td>Left and right border style of normal tabs</td>
<td><pre> {
//all css3 paramerers of 'color'
'borderColor': '#ffd3a6'
}</pre></td>
</tr>
<tr>
<td>series[0].bothSidesStyle.emphasis | Object</td>
<td>Left and right border style if enphasis tabs</td>
<td><pre> {
'borderColor': '#f6eb3f'
}</pre></td>
</tr>
<tr>
<td>series[0].name | String</td>
<td>Field name of data</td>
<td></td>
</tr>
<tr>
<td>itemGap | Number</td>
<td>Gap between tab and another</td>
<td></td>
</tr>
</table>


> 注：
>
> * 导航栏尚未绑定数据时，可以对series\[0\].data进行编辑；导航栏绑定数据后，series\[0\].data会自动生成相应信息，用户只可以对name值进行修改
> * textStyle两种状态下的文本样式均支持CSS3中的文本样式，命名采用驼峰命名方式，用户可按照规则添加其他文本样式




