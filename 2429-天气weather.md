# 天气\_Weather ![](/assets/Weather.png)

---

> ## 开发模式

### 参数配置列表

```
{
    'type': 'Weather',
    'weatherControlStyle': {
        'background': '#ccc'
    },
    'getWeather': {
        'width': '300px',
        'height': '300px',
        'isByCity': {
            'byCity': true,
            'city': '北京'
        },
        'isByCoordinates': {
            'byCooordinates': false,
            'longitude': '116.305145',
            'latitude': '39.982368'
        },
        'windStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'weatherStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'temperatureStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'timeStyle': {
            'textStyle': {
                'color': '#fff'
            }
        },
        'weekStyle': {
            'textStyle': {
                'color': '#fff'
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
	<td>Weather</td>
</tr>
<tr>
	<td>weatherControlStyle | Object</td>
	<td>Style of Weather Component</td>
	<td><pre> {
	//Background style, can be parameter of css3 'background'
	'background': '#ccc'
}</pre></td>
</tr>
<tr>
	<td>getWeather | Object</td>
	<td>Get weather infomation and style</td>
	<td><pre> {
	//Width of component, can be parameter of css3 'width'
	'width': '300px',
	//Height of component, can be parameter of css3 'height'
	'height': '300px',
	...
}</pre></td>
</tr>
<tr>
	<td>getWeather.isByCity | Object</td>
	<td>Get weather infomation by city name, attributes can be 'byCity' and 'city'</td>
	<td><pre> {
	//Whether or not to get weather infomation by city
	'byCity': 'true',
	//City name
	'city': '北京'
}</pre></td>
</tr>
<tr>
	<td>getWeather.isByCoordinates | Object</td>
	<td>Get weather infomation by coordinate, attributes can be 'byCoordinates', 'longitude' and 'latitude'</td>
	<td><pre> {
	//Whether or not to get weather infomation by coordinate
	'byCoordinates': 'true',
	//get longitude
	'longitude': '116.305145',
	//get latitude
	'latitude': '39.982368'
}</pre></td>
</tr>
<tr>
	<td>getWeather.windStyle | Object</td>
	<td>Infomation and style of wind</td>
	<td><pre> {
	//Content style
	'textStyle': {
		//Content color, can be parameter of css3 'color'
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.weatherStyle | Object</td>
	<td>Infomation and style of whether</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.temperatureStyle | Object</td>
	<td>Infomation and style of temperature</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.timeStyle | Object</td>
	<td>Infomation and style of time</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
<tr>
	<td>getWeather.weekStyle | Object</td>
	<td>Infomation and style of week</td>
	<td><pre> {
	'textStyle': {
		'color': '#fff'
	}
}</pre></td>
</tr>
</table>

> 注：
>
> * weatherControlStyle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他天气样式
> * getWeather.windStyle.textSryle、getWeather.weatherStyle.textSryle、getWeather.temperatureStyle.textSryle、getWeather.timeStyle.textSryle、getWeather.weekStyle.textSryle中的属性支持CSS3中的样式属性，命名采用驼峰命名方式，用户可按照规则添加其他天气信息样式



