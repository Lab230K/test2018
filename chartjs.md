inconclusive-stranger
ShowLive

README.md

Chart.js Starter
=================
​
🔗 [Chart.js documentation](https://chartjs.org)
​
This app uses [Chart.js](https://chartjs.org) (client-side) to display a bar chart and a pie chart showing world population by continent. Chart.js is a tool for creating interactive charts and graphs in the browser.
​
> [Check out the live-stream where we remix this app](https://www.youtube.com/watch?v=HGNFAlhp69o)
> [Read the blog post where we explain how this app works in detail](
​
## Getting started
​
First of all, remix this app! Remixing will create your own copy of the app that is unique to you -- any changes you make will only apply to your version. Make sure you change the description in your version so you remember what the app does when you're looking at it later
​
Here are some ideas for ways to customize this app:
1. Add your own data by changing the keys and values in the `data` object in `script.js`
2. Change the colors and label values of the charts within each `new Chart()` constructor
3. Add custom chart behavior using [Configurations](https://www.chartjs.org/docs/latest/configuration/)
4. Create a different [type of chart](https://www.chartjs.org/docs/latest/charts/) with the data.
​
## Code
​
The code powering this app is in `index.html`, `script.js`, and `style.css`.
​
### `index.html`
​
- The Chart.js JavaScript library is included in `head`
- `body` has two `div` elements with class `.chart-container`
- inside each `.chart-container` div is a `canvas` element with ID `#barChart` or `#pieChart`
  - Chart.js dynamically inserts a chart into a `canvas` element, which is why an empty `canvas` is added for each chart. The `div` wrapped around the `canvas` is there for styling purposes, as options for styling `canvas` elements with CSS are limited.
​
### `script.js`
​
- a `data` object is defined with countries as keys and population numbers as values
- a `countries` array is created from the keys of the `data` object
- a `populations` array is created from the values of the `data` object
- a bar chart is initialized and placed in the `barChart` canvas
  - type: bar chart
  - data: `countries` as labels (x-axis), `populations` as values (y-axis), make each bar in the bar chart red
  - options: have the y-axis start at 0
- a pie chart is initialized and placed in the `pieChart` canvas
  - type: pie chart
  - data: `countries` as labels (sections of the pie), `populations` as values (width of pie slices), each section has a different color
  
### `style.css`
​
- add a purple border around each `canvas`
- set a height, width, margin, and position for the `chart-container` to make charts responsive to different window sizes and platforms
​
​
Made by [Glitch](https://glitch.com/)
-------------------
​
\ ゜o゜)ノ
​
