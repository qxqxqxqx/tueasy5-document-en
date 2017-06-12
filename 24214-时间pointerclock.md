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
| clock | Object | √ |  |  | Style of clock |
| clock.clockAxis | Object | √ |  |  | Style of scale line |
| clock.clockAxis.axisLine | Object | √ |  |  | Style of circle line |
| clock.clockAxis.axisLine.show | Bool | √ | true |  | Whether or not to show circle line |
| clock.clockAxis.axisLine.lineStyle | Object | √ |  |  | Style of circle line |
| clock.clockAxis.axisLine.lineStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of circle line |
| clock.clockAxis.axisTick | Object | √ |  |  | Style of scale line |
| clock.clockAxis.axisTick.show | Bool | √ | true |  | Whether or not to show the scale line |
| clock.clockAxis.axisTick.lineStyle | Object | √ |  |  | The style of the scale line |
| clock.clockAxis.axisTick.lineStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of scale line |
| clock.clockAxis.axisText | Object | √ |  |  | Style of number |
| clock.clockAxis.axisText.textGap | String | √ | 5px |  | Gap between number and circle line |
| clock.clockAxis.axisText.textStyle | Object | √ |  |  | Text style of number |
| clock.clockAxis.axisText.textStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of number |
| clock.outerCircle | Object | √ |  |  | Style of outer circle |
| clock.outerCircle.show | Bool | √ | true |  | Whether or not to show the outer circle |
| clock.outerCircle.lineStyle | Object | √ |  |  | The style of the outer circle line |
| clock.outerCircle.lineStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of outer circle |
| clock.middleCircle | Object | √ |  |  | Style of middle circle |
| clock.middleCircle.show | Bool | √ | true |  | Whether or not to show the middle circle |
| clock.middleCircle.lineStyle | Object | √ |  |  | The style of the middle circle line |
| clock.middleCircle.lineStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of middle circle |
| clock.innerCircle | Object | √ |  |  | Style of inner circle |
| clock.innerCircle.show | Bool | √ | true |  | Whether or not to show inner circle |
| clock.innerCircle.lineStyle | Object | √ |  |  | Style of inner circle line |
| clock.innerCircle.lineStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of inner circle |
| clock.hand | Object | √ |  |  | Style of hand |
| clock.hand.clockHourHand | Object | √ |  |  | Color of hour hand |
| clock.hand.clockHourHand.handStyle | Object | √ |  |  | Style of hour handle |
| clock.hand.clockHourHand.handStyle.fill | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Fll color of hour handle |
| clock.hand.clockHourHand.handStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Border color of hour handle |
| clock.hand.clockHourHand.lineStyle | Object | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of the rest part of hour handle |
| clock.hand.clockMinuteHand | Object | √ |  |  | Style of minute hand |
| clock.hand.clockMinuteHand.handStyle | Object | √ |  |  | Style of minute handle |
| clock.hand.clockMinuteHand.handStyle.fill | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Fill color of minute handle |
| clock.hand.clockMinuteHand.handStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Border color of minute handle |
| clock.hand.clockMinuteHand.lineStyle | Object | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of the rest part of minute handle |
| clock.hand.clockSecondHand | Object | √ |  |  | Style of second hand |
| clock.hand.clockSecondHand.handStyle | Object | √ |  |  | Style of second handle |
| clock.hand.clockSecondHand.handStyle.fill | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Fill color of minute handle |
| clock.hand.clockSecondHand.lineStyle | Object | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Color of the rest part of second handle |
| clock.aloneArc | Object | √ |  |  | Single arc to decorate the clock |
| clock.aloneArc.show | Bool | √ | true |  | Whether or not to show the single arc |
| clock.aloneArc.lineStyle | Object | √ |  |  | Style of the single arc |
| clock.aloneArc.lineStyle.fill | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Fill color of the single arc |
| clock.aloneArc.lineStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Border color of the single arc |
| clock.symmetryArc | Object | √ |  |  | Symmetrical arcs to decorate the clock |
| clock.symmetryArc.show | Bool | √ | true |  | Whether or not to show the symmetrical arcs |
| clock.symmetryArc.lineStyle | Object | √ |  |  | Style of the symmetrical arcs |
| clock.symmetryArc.lineStyle.fill | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Fill color of the symmetrical arcs |
| clock.symmetryArc.lineStyle.stroke | String | √ | \#5a9cc7 | Color parameters including Color Name, HEX, RGB, RGBA, HSL, HSLA, transparent | Border color of the symmetricle arcs |



