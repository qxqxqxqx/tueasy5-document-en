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
| [grid](#grid) | Array\(Object\) | √ |  |  | Cartesian grid within a cartesian coortnate system |
| [tooltip](#tooltip) | Object | √ |  |  | 提示框，鼠标悬浮交互式时的信息提示 |
| [xAxis](#xaxis) | Array\(Object\) | √ |  |  | 直角坐标系中横轴数组 |
| yAxis | Array\(Object\) | √ |  |  | 直角坐标系中纵轴数组 |
| series | Array\(Object\) | √ |  |  | 该图表的详细配置 |

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

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| grid\[0\].top | Number | √ | 10 |  | 直角坐标系内绘图网格左上角横坐标，数值单位px |
| grid\[0\].right | Number | √ | 50 |  | 直角坐标系内绘图网格左上角纵坐标，数值单位px |
| grid\[0\].bottom | Number | √ | 20 |  | 直角坐标系内绘图网格右下角纵坐标，数值单位px |
| grid\[0\].left | Number | √ | 50 |  | 直角坐标系内绘图网格右下角横坐标，数值单位px |
| grid\[0\].bgStyle | Object | √ |  |  | 直角坐标系内平面样式 |
| grid\[0\].bgStyle.normal | Object | √ |  |  | **未选中**状态的平面样式 |
| grid\[0\].bgStyle.normal.fill | String | √ | rgba\(0,0,0,0\) |  | **未选中**状态的平面填充颜色 |
| grid\[0\].bgStyle.emphasis | Object | √ |  |  | **选中**状态的平面样式 |
| grid\[0\].bgStyle.emphasis.fill | String | √ | rgba\(0,0,0,0\) |  | **选中**状态的平面填充颜色 |

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

| 配置项 | 类型 | 必填 | 默认值 | 可选参数 | 功能/备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| xAxis\[0\].type | String | √ | linear | category、linear |  |
| xAxis\[0\].inverse | Boolean | √ | false |  | 是否沿水平方向反转图表 |
| xAxis\[0\].axisLine | Object | √ |  |  | 水平坐标轴线 |
| xAxis\[0\].axisLine.show | Boolean | √ | false |  | 是否显示水平坐标轴线。 |
| xAxis\[0\].axisLine.lineStyle | Object | √ |  |  | 水平坐标轴线样式 |
| xAxis\[0\].axisLine.lineStyle.stroke | String | √ |  |  | 水平坐标轴线颜色 |
| xAxis\[0\].axisLine.lineStyle.stroke-width | String | √ | 2 |  | 水平坐标轴线宽度 |
| xAxis\[0\].axisLabel | Object | √ |  |  | 水平坐标轴文本标签 |
| xAxis\[0\].axisLabel.show | Boolean | √ | false |  | 是否显示水平坐标轴文本标签 |
| xAxis\[0\].axisLabel.interval | String \| Number | √ | auto |  | 水平坐标轴文本标签间隔。auto-自动隐藏显示不下的；0-全部显示 |
| xAxis\[0\].axisLabel.inside | Boolean | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.rotate | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.margin | Number | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.formatter | String \| Function | -- | -- | -- | -- |
| xAxis\[0\].axisLabel.textStyle | Object | √ |  |  | 水平坐标轴文本标签中的文本样式 |
| xAxis\[0\].axisLabel.textStyle.font-size | Number | √ | 12 |  | 水平坐标轴文本标签中的文本大小 |
| xAxis\[0\].axisLabel.textStyle.font-style | String | √ | normal |  | 水平坐标轴文本标签中的文本样式 |
| xAxis\[0\].axisLabel.textStyle.font-weight | String | √ | normal |  | 水平坐标轴文本标签中的文本粗细 |
| xAxis\[0\].axisLabel.textStyle.font-family | String | √ | sans-serif |  | 水平坐标轴文本标签中的文本字体 |
| xAxis\[0\].axisLabel.textStyle.fill | String | √ | \#fff |  | 水平坐标轴文本标签中的文本颜色 |
| xAxis\[0\].axisTick | Object | √ |  |  | 水平坐标轴刻度线 |
| xAxis\[0\].axisTick.show | Boolean | √ | false |  | 是否显示水平坐标轴刻度线 |
| xAxis\[0\].axisTick.symbol | String | √ | line |  | 水平坐标轴刻度线符号 |
| xAxis\[0\].axisTick.inside | Boolean | √ | false |  | 水平坐标轴刻度线是否位于坐标轴内侧 |
| xAxis\[0\].axisTick.length | Number | √ | 10 |  | 水平坐标轴刻度线的高度 |
| xAxis\[0\].axisTick.symbolStyle | Object | √ |  |  | 水平坐标轴刻度线符号样式 |
| xAxis\[0\].axisTick.symbolStyle.stroke | String | √ | \#fff |  | 水平坐标轴刻度线符号颜色 |
| xAxis\[0\].axisTick.symbolStyle.stroke-width | Number | √ | 1 |  | 水平坐标轴刻度线符号宽度 |
| xAxis\[0\].splitLine | Object | √ |  |  | 水平坐标轴的分割区域 |
| xAxis\[0\].splitLine.show | Boolean | √ | true |  | 是否显示水平坐标轴的分割区域线 |
| xAxis\[0\].splitLine.lineStyle | Object | √ |  |  | 水平坐标轴的分割区域线样式 |
| xAxis\[0\].splitLine.lineStyle.stroke | String | √ | \#0f0 |  | 水平坐标轴的分割区域线颜色 |
| xAxis\[0\].splitLine.lineStyle.stroke-width | Number | √ | 1 |  | 水平坐标轴的分割区域线粗细 |
| xAxis\[0\].splitLine.lineStyle.stroke-dasharray | Array\(Number\) | √ | \[1 0\] | 支持SVG stroke-dasharray属性的参数值 | 水平坐标轴的分割区域线类型 |
| xAxis\[0\].position | String | √ | bottom | bottom、left、right、top | 水平坐标轴的位置 |
| xAxis\[0\].min | Number | √ | 0 |  | 水平坐标轴的最小值 |
| xAxis\[0\].max | Number | √ | 1500 |  | 水平坐标轴的最大值 |
| xAxis\[0\].name | String | -- | -- | -- | 水平坐标轴的自定义名称 |
| xAxis\[0\].nameLocation | String | -- | -- | center、end、start | 水平坐标轴的自定义名称位置 |
| xAxis\[0\].nameGap | Number | -- | -- | -- | 水平坐标轴名称距离坐标轴的距离 |
| xAxis\[0\].data | Array\(String\) |  |  |  | 水平坐标轴的离散数值 |
| xAxis\[0\].boundaryGap | Number | -- | -- | -- | 水平坐标轴两端留白的大小 |
| xAxis\[0\].splitNumber | Number | √ | 5 |  | 水平坐标轴分割的段数 |
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
| series\[0\].name | String | √ |  |  | 系列数据的名称，不可重复 |
| series\[0\].type | String | √ | tickbar |  | 系列数据显示的类型--tickBar柱形图/条形图 |
| series\[0\].coordinateSystem | String | √ | cartesian2d |  | 图表坐标类型--cartesian2d2D坐标类型 |
| series\[0\].data | Array\(Number\) | √ |  |  | 系列数据的数据值 |
| series\[0\].clipPath | Object | √ |  |  | 柱形图/条形图中的小单元 |
| series\[0\].clipPath.symbol | String | √ | rect | circle、person、rect | 柱形图/条形图中的小单元图形样式。circle为圆形，person为人形，rect为圆形 |
| series\[0\].clipPath.symbolGap | Number | √ | 0.1 |  | 柱形图/条形图中的小单元间距 |
| series\[0\].clipPath.symbolNumber | Number | √ | 15 |  | 一行柱形/条形中的小单元数目 |
| series\[0\].clipPath.showBack | Boolean | √ | true |  | 是否显示无值的小单元部分 |
| series\[0\].symbolStyle | Object | √ |  |  | 小单元样式 |
| series\[0\].symbolStyle.normal | Object | √ |  |  | 小单元**未选中**状态样式 |
| series\[0\].symbolStyle.normal.fill | String | √ |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |



