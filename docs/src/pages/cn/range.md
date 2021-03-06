# Range

> 滑块，支持自定义步长、区间等。

-------------

## 引入

```javascript
import { yepRange } from 'YepUI';

Vue.use(yepRange);
```

## 例子

将一个本地变量与 `range` 的 `value` 属性同步即可实现双向绑定

```html
<yep-range value.sync="rangeValue"></yep-range>
```

更多的配置项


```html
<yep-range :value.sync="rangeValue"
	:min="min"
  	:max="max"
   	:step="step"
   	:bar-height="barHeight"
   	:bar-color="barColor"
   	:disabled="disabled">
</yep-range>
```

可在滑块两侧显示文字

```html
<yep-range value.sync="rangeValue">
	<div slot="start">0</div>
	<div slot="end">100</div>
</yep-range>
```

## API
| 参数 | 说明 | 类型 | 可选值 | 默认值 |
|------|-------|---------|-------|--------|
| value | 滑块的值 | Number | | |
| min | 最小值 | Number | | 0 |
| max | 最大值 | Number | | 100 |
| step | 步长 | Number | | 1 |
| disabled | 是否禁用 | Boolean | | false |
| barHeight | 滑槽的线宽（像素） | Number | | 1 |
| barColor | 滑槽的色值 | Number | | #26a2ff |

## Slot
| name | 描述 |
|------|--------|
| start | 滑块左侧 DOM |
| end | 滑块右侧 DOM |
