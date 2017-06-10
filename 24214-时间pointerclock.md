# 时间\_PionterClock ![](/assets/PointerClock.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'clock': {
        'clockAxis': {
            'axisLine': {
                'show': true,
                'lineStyle': {
                    'stroke': '#5a9cc7'
                }
            },
            'axisTick': {
                'show': true,
                'lineStyle': {
                    'stroke': '#5a9cc7'
                }
            },
            'axisText': {
                'textGap': 5,
                'textStyle': {
                    'stroke': '#5a9cc7'
                }
            }
        },
        'outerCircle': {
            'show': true,
            'lineStyle': {
                'fill': '#5a9cc7'
            }
        },
        'middleCircle': {
            'show': true,
            'lineStyle': {
                'stroke': '#5a9cc7'
            }
        },
        'innerCircle': {
            'show': true,
            'lineStyle': {
                'stroke': '#5a9cc7'
            }
        },
        'hand': {
            'clockHourHand': {
                'handStyle': {
                    'fill': '#5a9cc7',
                    'stroke': '#5a9cc7'
                },
                'lineStyle': {
                    'stroke': '#5a9cc7'
                }
            },
            'clockMinuteHand': {
                'handStyle': {
                    'fill': '#5a9cc7',
                    'stroke': '#5a9cc7'
                },
                'lineStyle': {
                    'fill': '#5a9cc7'
                }
            },
            'clockSecondHand': {
                'handStyle': {
                    'fill': '#5a9cc7'
                },
                'lineStyle': {
                    'fill': '#5a9cc7'
                }
            }
        },
        'aloneArc': {
            'show': true,
            'lineStyle': {
                'fill': '#5a9cc7',
                'stroke': '#5a9cc7'
            }
        },
        'symmetryArc': {
            'show': true,
            'lineStyle': {
                'fill': '#5a9cc7',
                'stroke': '#5a9cc7'
            }
        }

    },
    'series': [
        {
            'type': 'PointerClock'
        }
    ]
}
```

### 参数字段说明

![](/assets/pointerClock01.png)

| Configuration item | Type | Required | Default | Optional parameters | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| clock | Object | √ |  |  | The style of the clock |
| clock.clockAxis | Object | √ |  |  | The style of the scale line |
| clock.clockAxis.axisLine | Object | √ |  |  | The style of the circle line |
| clock.clockAxis.axisLine.show | Bool | √ | true |  | Whether or not to show the circle line |
| clock.clockAxis.axisLine.lineStyle | Object | √ |  |  | The style of the circle line |
| clock.clockAxis.axisLine.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the circle line |
| clock.clockAxis.axisTick | Object | √ |  |  | The style of the scale line |
| clock.clockAxis.axisTick.show | Bool | √ | true |  | Whether or not to show the scale line |
| clock.clockAxis.axisTick.lineStyle | Object | √ |  |  | The style of the scale line |
| clock.clockAxis.axisTick.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The  color of the scale line |
| clock.clockAxis.axisText | Object | √ |  |  | The style of the number |
| clock.clockAxis.axisText.textGap | String | √ | 5px |  | The gap between the number and the circle line |
| clock.clockAxis.axisText.textStyle | Object | √ |  |  | The text style of the number |
| clock.clockAxis.axisText.textStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the number |
| clock.outerCircle | Object | √ |  |  | The style of the outer circle |
| clock.outerCircle.show | Bool | √ | true |  | Whether or not to show the outer circle |
| clock.outerCircle.lineStyle | Object | √ |  |  | The style of the outer circle line |
| clock.outerCircle.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the outer circle |
| clock.middleCircle | Object | √ |  |  | The style of the middle circle |
| clock.middleCircle.show | Bool | √ | true |  | Whether or not to show the middle circle |
| clock.middleCircle.lineStyle | Object | √ |  |  | The style of the middle circle line |
| clock.middleCircle.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the middle circle |
| clock.innerCircle | Object | √ |  |  | The style of the inner circle |
| clock.innerCircle.show | Bool | √ | true |  | Whether or not to show the inner circle |
| clock.innerCircle.lineStyle | Object | √ |  |  | The style of the inner circle line |
| clock.innerCircle.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the inner circle |
| clock.hand | Object | √ |  |  | The style of the hand |
| clock.hand.clockHourHand | Object | √ |  |  | The color of the hour hand |
| clock.hand.clockHourHand.handStyle | Object | √ |  |  | The style of the hour handle |
| clock.hand.clockHourHand.handStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The fill color of the hour handle |
| clock.hand.clockHourHand.handStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The border color of the hour handle |
| clock.hand.clockHourHand.lineStyle | Object | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the rest part of the hour handle |
| clock.hand.clockMinuteHand | Object | √ |  |  | The style of the minute hand |
| clock.hand.clockMinuteHand.handStyle | Object | √ |  |  | The style of the minute handle |
| clock.hand.clockMinuteHand.handStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The fill color of the minute handle |
| clock.hand.clockMinuteHand.handStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The border color of the minute handle |
| clock.hand.clockMinuteHand.lineStyle | Object | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the rest part of the minute handle |
| clock.hand.clockSecondHand | Object | √ |  |  | The style of the  second hand |
| clock.hand.clockSecondHand.handStyle | Object | √ |  |  | The style of the second handle |
| clock.hand.clockSecondHand.handStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The fill color of the minute handle |
| clock.hand.clockSecondHand.lineStyle | Object | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The color of the rest part of the second handle |
| clock.aloneArc | Object | √ |  |  | The single arc to decorate the clock |
| clock.aloneArc.show | Bool | √ | true |  | Whether or not to show the single arc |
| clock.aloneArc.lineStyle | Object | √ |  |  | The style of the single arc |
| clock.aloneArc.lineStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The fill color of the single arc |
| clock.aloneArc.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The border color of the single arc |
| clock.symmetryArc | Object | √ |  |  | The symmetrical arcs to decorate the clock |   |
| clock.symmetryArc.show | Bool | √ | true |  | Whether or not to show the symmetrical arcs |
| clock.symmetryArc.lineStyle | Object | √ |  |  | The style of the symmetrical arcs |
| clock.symmetryArc.lineStyle.fill | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The fill color of the symmetrical arcs |
| clock.symmetryArc.lineStyle.stroke | String | √ | \#5a9cc7 | 支持CSS3中颜色的参数值，包括Color Name\(颜色名称\)、HEX、RGB、RGBA、HSL、HSLA、transparent | The border color of the symmetricle arcs |



