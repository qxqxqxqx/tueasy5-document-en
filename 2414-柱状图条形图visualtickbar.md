# 开发模式——通用参数

---

针对柱状图/条形图/折线图/散点图/面积图这类具有坐标轴的2D图表的通用参数

### 整体参数列表

```
{
    'color': [...],
    'grid': [...],
    'tooltip': [...],
    'xAxis': [...],
    'yAxis': [...],
    'series': [...]
}
```

### 整体参数说明

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| color | Array\(String\) | √ |  |  | The default color configuration list for the data item,the array element is a hexadecimal representation of the color |
| [grid](#grid) | Array\(Object\) | √ |  |  | Drawing grid within a Cartesian coortnate system |
| [tooltip](#tooltip) | Object | √ |  |  | Message box with interactive information when the mouse is suspended |
| [xAxis](#xaxis) | Array\(Object\) | √ |  |  | The horizontal axis array of Cartesian coordinate system |
| yAxis | Array\(Object\) | √ |  |  | The vertical axis array of Cartesian coordinate system |
| series | Array\(Object\) | √ |  |  | Detail configuration of this chart |

* ### grid

**参数配置列表**

```
'grid': [
        {
            'top': 10,
            'right': 50,
            'bottom': 20,
            'left': 50,
            'bgStyle': {
                'normal': {
                    'fill': 'rgba(0,0,0,0)'
                },
                'emphasis': {
                    'fill': 'rgba(0,0,0,0)'
                }
            }
        }
    ]
```

**参数字段说明**

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| grid\[0\].top | Number | √ | 10 |  | The abscissa of the upper left corner in the drawing grid, the numerical unit is px |
| grid\[0\].right | Number | √ | 50 |  | The ordinate of the upper left corner in the drawing grid, the numerical unit is px |
| grid\[0\].bottom | Number | √ | 20 |  | The ordinate of bottom right corner in the drawing grid, the numerical unit is px |
| grid\[0\].left | Number | √ | 50 |  | The abscissa of bottom right corner in the drawing grid, the numerical unit is px |
| grid\[0\].bgStyle | Object | √ |  |  | The background style of the Cartesian coordinate system |
| grid\[0\].bgStyle.normal | Object | √ |  |  | The background style of the **unselected state** |
| grid\[0\].bgStyle.normal.fill | String | √ | rgba\(0,0,0,0\) |  | The background color of the **unselected state** |
| grid\[0\].bgStyle.emphasis | Object | √ |  |  | The background color of the **selected state** |
| grid\[0\].bgStyle.emphasis.fill | String | √ | rgba\(0,0,0,0\) |  | The background color of the **selected state** |

* ### tooltip

**参数配置列表**

```
'tooltip': {
        'show': true,
        'style': {
            'border-color': '#cc0',
            'border-radius': '5',
            'border-width': '2',
            'border-style': 'solid',
            'width': '100',
            'height': '60',
            'text-align': 'center',
            'line-height': '60',
            'pointer-events': 'none',
            'background-color': 'rgba(255, 255, 255, 0.7)'
        },
        'formatter': function formatter(param) {

            return param.dataIndex + ': ' + param.value;
        },
        'position': function position() {

            return [20, 10];
        }
    }
```

**参数字段说明**

|  |  |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  |  |  |  |  |  |

* ### xAxis

**参数配置列表**

```
'xAxis': [
        {
            'type': 'linear',
            'inverse': false,
            'axisLine': {
                'show': false,
                'lineStyle': {
                    'stroke': 'yellow',
                    'stroke-width': '2'
                }
            },
            'axisLabel': {
                'show': false,
                'interval': 'auto',
                'inside': false,
                'rotate': 0,
                'margin': 8,
                'formatter': null,
                'textStyle': {
                    'font-size': 12,
                    'font-style': 'normal',
                    'font-weight': 'normal',
                    'font-family': 'sans-serif',
                    'fill': '#fff'
                }
            },
            'axisTick': {
                'show': false,
                'symbol': 'line',
                'inside': false,
                'length': 10,
                'symbolStyle': {
                    'stroke': '#fff',
                    'stroke-width': 1
                }
            },
            'splitLine': {
                'show': false,
                'lineStyle': {
                    'fill': 'none',
                    'stroke': '#0f0',
                    'stroke-width': 1,
                    'type': 'dashed'
                }
            },
            'position': 'bottom',
            'min': 0,
            'max': 1500,
            'name': '',
            'nameLocation': '',
            'nameGap': '',
            'data': '',
            'boundaryGap': 1,
            'splitNumber': 5,
            'splitTicks': [

            ],
            'splitArea': {
                'show': true,
                'areaStyle': {

                }
            }
        }
    ],
```

**参数字段说明**

| Configuration item | Type | Required | Default | Optional parameter | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| xAxis\[0\].type | String | √ | linear | category、linear |  |
| xAxis\[0\].inverse | Boolean | √ | false |  | Whether or not to reverse the chart in the horizontal direction |
| xAxis\[0\].axisLine | Object | √ |  |  | Horizontal axis |
| xAxis\[0\].axisLine.show | Boolean | √ | false |  | Whether or not to show the horizontal axis |
| xAxis\[0\].axisLine.lineStyle | Object | √ |  |  | The style of the horizontal axis |
| xAxis\[0\].axisLine.lineStyle.stroke | String | √ |  |  | The color of the horizontal axis |
| xAxis\[0\].axisLine.lineStyle.stroke-width | String | √ | 2 |  | The width of the horizontal axis |
| xAxis\[0\].axisLabel | Object | √ |  |  | The text label of the horizontal axis |
| xAxis\[0\].axisLabel.show | Boolean | √ | false |  | Whether or not to show the text label of the horizontal axis |
| xAxis\[0\].axisLabel.interval | String \| Number | √ | auto |  | The gap of the text labels. 'auto' means automatically hide the overflow ones; '0' means show all |
| xAxis\[0\].axisLabel.inside | Boolean | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.rotate | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.margin | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.formatter | String \| Function | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.textStyle | Object | √ |  |  | The text style of the text label |
| xAxis\[0\].axisLabel.textStyle.font-size | Number | √ | 12 |  | The fontsize of the text label |
| xAxis\[0\].axisLabel.textStyle.font-style | String | √ | normal |  | The fontStyle of the text label |
| xAxis\[0\].axisLabel.textStyle.font-weight | String | √ | normal |  | The fontWeight of the text label |
| xAxis\[0\].axisLabel.textStyle.font-family | String | √ | sans-serif |  | The fontFamily of the text label |
| xAxis\[0\].axisLabel.textStyle.fill | String | √ | \#fff |  | The text color of the text label |
| xAxis\[0\].axisTick | Object | √ |  |  | The scale line of the horizontal axis |
| xAxis\[0\].axisTick.show | Boolean | √ | false |  | Whether or not to show the scale line |
| xAxis\[0\].axisTick.symbol | String | √ | line |  | The symbol of the scale line |
| xAxis\[0\].axisTick.inside | Boolean | √ | false |  | Whether the scale line is inside of the horizontal axis or not |
| xAxis\[0\].axisTick.length | Number | √ | 10 |  | The height of the scale line |
| xAxis\[0\].axisTick.symbolStyle | Object | √ |  |  | The style of the scale line symbol |
| xAxis\[0\].axisTick.symbolStyle.stroke | String | √ | \#fff |  | The color of the scale line symbol |
| xAxis\[0\].axisTick.symbolStyle.stroke-width | Number | √ | 1 |  | The width of the scale line symbol |
| xAxis\[0\].splitLine | Object | √ |  |  | The split line of the horizontal axis |
| xAxis\[0\].splitLine.show | Boolean | √ | true |  | Whether or not to show the split line |
| xAxis\[0\].splitLine.lineStyle | Object | √ |  |  | The style of the split line |
| xAxis\[0\].splitLine.lineStyle.stroke | String | √ | \#0f0 |  | The color of the split line |
| xAxis\[0\].splitLine.lineStyle.stroke-width | Number | √ | 1 |  | The width of the split line |
| xAxis\[0\].splitLine.lineStyle.stroke-dasharray | Array\(Number\) | √ | \[1 0\] | SVG stroke-dasharray parameter supported | The type of the split line |
| xAxis\[0\].position | String | √ | bottom | bottom、left、right、top | The position of the horizontal axis |
| xAxis\[0\].min | Number | √ | 0 |  | The minimum value of the horizontal axis |
| xAxis\[0\].max | Number | √ | 1500 |  | The maximum value of the horizontal axis |
| xAxis\[0\].name | String | -- | -- | -- | The name of the horizontal axis |
| xAxis\[0\].nameLocation | String | -- | -- | center、end、start | The position of the horizontal axis name |
| xAxis\[0\].nameGap | Number | -- | -- | -- | The gap between the name and the horizontal axis |
| xAxis\[0\].data | Array\(String\) |  |  |  | The discrete values of the horizontal value |
| xAxis\[0\].boundaryGap | Number | -- | -- | -- | The gaps of both ends blank |
| xAxis\[0\].splitNumber | Number | √ | 5 |  | Number of the horizontal divided |
| xAxis\[0\].splitTicks | Array | -- | -- | -- | -- |
| xAxis\[0\].splitArea | Object | -- | -- | -- | -- |
| xAxis\[0\].splitArea.show | Boolean | -- | -- | -- |  |
| xAxis\[0\].splitArea.areaStyle | Object | -- | -- | -- | -- |

* ### yAxis

yAxis的配置与xAxis的配置相同

* ### series

**参数配置列表**

```
'series': [
        {
            'name': 'Apple',
            'type': 'tickbar',
            'coordinateSystem': 'cartesian2d',
            'data': [
                900,
                600,
                1100,
                800,
                1300
            ],
            'clipPath': {
                'symbol': 'rect',
                'symbolGap': 0.1,
                'symbolNumber': 15,
                'showBack': true
            },
            'symbolStyle': {
                'normal': {
                    'fill': 'rgb(41, 237, 138)',
                    'borderColor': 'rgba(0, 0, 0, 0)',
                    'borderWidth': 0,
                    'borderType': 'none',
                    'barBorderRadius': 0
                },
                'emphasis': {
                    'fill': 'rgb(248, 234, 95)'
                },
                'backgroundColor': 'rgb(212, 251, 241)'
            },
            'label': {
                'position': 'maxRight',
                'textStyle': {
                    'fill': 'rgb(122, 122, 122)',
                    'fontSize': 12,
                    'fontStyle': 'normal',
                    'fontWeight': 'normal',
                    'fontFamily': 'sans-serif',
                    'font-size': '17px',
                    'pointer-events': 'none'
                },
                'show': true,
                'symbol': 'text',
                'offsetX': 10,
                'offsetY': 0,
                'formatter': function formatter(param) {

                    return param.value;
                }
            },
            'barWidth': 30,
            'barGap': 10
        }
    ]
```

**参考字段说明**

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| series\[0\].name | String | √ |  |  | The name of the data which can not be repeated |
| series\[0\].type | String | √ | tickbar |  | The chart type base on the data,E.g: tickbar means bar chart |
| series\[0\].coordinateSystem | String | √ | cartesian2d |  | The type of the coordinate system |
| series\[0\].data | Array\(Number\) | √ |  |  | The data values |
| series\[0\].clipPath | Object | √ |  |  | The minimum unit of the bar chart |
| series\[0\].clipPath.symbol | String | √ | rect | circle、person、rect | The type of the bar chart unit |
| series\[0\].clipPath.symbolGap | Number | √ | 0.1 |  | The  gaps between units |
| series\[0\].clipPath.symbolNumber | Number | √ | 15 |  | The number of the units |
| series\[0\].clipPath.showBack | Boolean | √ | true |  | Whether or not to show the units which has no value |
| series\[0\].symbolStyle | Object | √ |  |  | The style of the units |
| series\[0\].symbolStyle.normal | Object | √ |  |  | The style of the units which are unselected |
| series\[0\].symbolStyle.normal.fill | String | √ |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



