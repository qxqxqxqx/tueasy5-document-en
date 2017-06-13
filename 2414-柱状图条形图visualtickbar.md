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
| color | Array\(String\) | √ |  |  | The default color configuration list for the data item,the array element is color of the hexadecimal representation |
| [grid](#grid) | Array\(Object\) | √ |  |  | Drawing grid within a Cartesian coortnate system |
| [tooltip](#tooltip) | Object | √ |  |  | Message box with interactive information when the mouse is suspending |
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
| grid\[0\].top | Number | √ | 10 |  | Abscissa of the upper left corner in drawing grid, in px |
| grid\[0\].right | Number | √ | 50 |  | Ordinate of the upper left corner in drawing grid, in px |
| grid\[0\].bottom | Number | √ | 20 |  | Ordinate of bottom right corner in drawing grid, in px |
| grid\[0\].left | Number | √ | 50 |  | Abscissa of bottom right corner in drawing grid, in px |
| grid\[0\].bgStyle | Object | √ |  |  | Background style of Cartesian coordinate system |
| grid\[0\].bgStyle.normal | Object | √ |  |  | Background style of **unselected state** |
| grid\[0\].bgStyle.normal.fill | String | √ | rgba\(0,0,0,0\) |  | Background color of **unselected state** |
| grid\[0\].bgStyle.emphasis | Object | √ |  |  | Background color of **selected state** |
| grid\[0\].bgStyle.emphasis.fill | String | √ | rgba\(0,0,0,0\) |  | Background color of **selected state** |

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
| xAxis\[0\].inverse | Boolean | √ | false |  | Whether or not to reverse the chart in horizontal direction |
| xAxis\[0\].axisLine | Object | √ |  |  | Horizontal axis |
| xAxis\[0\].axisLine.show | Boolean | √ | false |  | Whether or not to show horizontal axis |
| xAxis\[0\].axisLine.lineStyle | Object | √ |  |  | Style of horizontal axis |
| xAxis\[0\].axisLine.lineStyle.stroke | String | √ |  |  | Color of horizontal axis |
| xAxis\[0\].axisLine.lineStyle.stroke-width | String | √ | 2 |  | Width of horizontal axis |
| xAxis\[0\].axisLabel | Object | √ |  |  | Text label of horizontal axis |
| xAxis\[0\].axisLabel.show | Boolean | √ | false |  | Whether or not to show text label of horizontal axis |
| xAxis\[0\].axisLabel.interval | String \| Number | √ | auto |  | Gap between text labels. 'auto' means to automatically hide overflow ones; '0' means to show all |
| xAxis\[0\].axisLabel.inside | Boolean | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.rotate | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.margin | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.formatter | String \| Function | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.textStyle | Object | √ |  |  | Text style of text label |
| xAxis\[0\].axisLabel.textStyle.font-size | Number | √ | 12 |  | Fontsize of text label |
| xAxis\[0\].axisLabel.textStyle.font-style | String | √ | normal |  | FontStyle of text label |
| xAxis\[0\].axisLabel.textStyle.font-weight | String | √ | normal |  | FontWeight of text label |
| xAxis\[0\].axisLabel.textStyle.font-family | String | √ | sans-serif |  | FontFamily of text label |
| xAxis\[0\].axisLabel.textStyle.fill | String | √ | \#fff |  | Text color of text label |
| xAxis\[0\].axisTick | Object | √ |  |  | Scale line of horizontal axis |
| xAxis\[0\].axisTick.show | Boolean | √ | false |  | Whether or not to show scale line |
| xAxis\[0\].axisTick.symbol | String | √ | line |  | Symbol of scale line |
| xAxis\[0\].axisTick.inside | Boolean | √ | false |  | Whether scale line is inside of horizontal axis or not |
| xAxis\[0\].axisTick.length | Number | √ | 10 |  | Height of scale line |
| xAxis\[0\].axisTick.symbolStyle | Object | √ |  |  | Style of scale line symbol |
| xAxis\[0\].axisTick.symbolStyle.stroke | String | √ | \#fff |  | Color of scale line symbol |
| xAxis\[0\].axisTick.symbolStyle.stroke-width | Number | √ | 1 |  | Width of scale line symbol |
| xAxis\[0\].splitLine | Object | √ |  |  | Split line of horizontal axis |
| xAxis\[0\].splitLine.show | Boolean | √ | true |  | Whether or not to show split line |
| xAxis\[0\].splitLine.lineStyle | Object | √ |  |  | Style of split line |
| xAxis\[0\].splitLine.lineStyle.stroke | String | √ | \#0f0 |  | Color of split line |
| xAxis\[0\].splitLine.lineStyle.stroke-width | Number | √ | 1 |  | Width of split line |
| xAxis\[0\].splitLine.lineStyle.stroke-dasharray | Array\(Number\) | √ | \[1 0\] | SVG stroke-dasharray parameter supported | Type of split line |
| xAxis\[0\].position | String | √ | bottom | bottom、left、right、top | Position of horizontal axis |
| xAxis\[0\].min | Number | √ | 0 |  | Minimum value of horizontal axis |
| xAxis\[0\].max | Number | √ | 1500 |  | Maximum value of horizontal axis |
| xAxis\[0\].name | String | -- | -- | -- | Name of horizontal axis |
| xAxis\[0\].nameLocation | String | -- | -- | center、end、start | Position of horizontal axis name |
| xAxis\[0\].nameGap | Number | -- | -- | -- | Gap between name and horizontal axis |
| xAxis\[0\].data | Array\(String\) |  |  |  | Discrete values of horizontal value |
| xAxis\[0\].boundaryGap | Number | -- | -- | -- | Gaps of both ends blank |
| xAxis\[0\].splitNumber | Number | √ | 5 |  | Number of horizontal dividing lines |
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
| series\[0\].name | String | √ |  |  | Name of the data which can not be repeated |
| series\[0\].type | String | √ | tickbar |  | Chart type base on the data,E.g: tickbar means bar chart |
| series\[0\].coordinateSystem | String | √ | cartesian2d |  | Type of the coordinate system |
| series\[0\].data | Array\(Number\) | √ |  |  | Data values |
| series\[0\].clipPath | Object | √ |  |  | Minimum unit of the bar chart |
| series\[0\].clipPath.symbol | String | √ | rect | circle、person、rect | Type of the bar chart unit |
| series\[0\].clipPath.symbolGap | Number | √ | 0.1 |  | Gaps between units |
| series\[0\].clipPath.symbolNumber | Number | √ | 15 |  | Number of the units |
| series\[0\].clipPath.showBack | Boolean | √ | true |  | Whether or not to show the units which has no value |
| series\[0\].symbolStyle | Object | √ |  |  | Style of the units |
| series\[0\].symbolStyle.normal | Object | √ |  |  | Style of the units which are unselected |
| series\[0\].symbolStyle.normal.fill | String | √ |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



