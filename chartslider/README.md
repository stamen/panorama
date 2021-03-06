## ChartSlider

An interactive overlay that can be applied over other charts, that enables selection along the x-axis.

Part of the [`@stamen/panorama`](https://www.npmjs.com/package/@stamen/panorama) toolkit.

<img src='https://cdn0.iconfinder.com/data/icons/feather/96/circle-check-32.png'>

#### Usage
```js
import React from 'react';
import ReactDOM from 'react-dom';
import { ChartSlider } from '@stamen/chartslider';

let chartSliderConfig = {
  width: 600,
  height: 200,

  // Optionally specify custom margins
  margin: { top: 10, right: 10, bottom: 10, left: 10 },

  // Optionally specify a custom scale
  scale: d3.scale.linear()
    .domain([minValue, maxValue]),

  selectedValue: currentValue,
  onClickOrMove: this.onValueSelected
};

ReactDOM.render(<ChartSlider {...chartSliderConfig}/>, document.body);
```
