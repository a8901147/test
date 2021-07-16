# test

https://css-tricks.com/making-a-bar-chart-with-css-grid/

.chart {
  display: grid;
  /* grid-template-columns: repeat(12, 1fr); */
  grid-template-rows: repeat(100, 1fr);
  grid-column-gap: 5px;
  height: 70vh;
  width: 70vw;
  padding: 5px 10px;
  margin: auto;
}

import classes from "./Chart.module.css";
import Bar from "./Bar";

function Chart() {
  return (
    <div className={classes.chart}>
      <Bar></Bar>
      <Bar></Bar>
      <Bar></Bar>
      <Bar></Bar>
      <Bar></Bar>
      <Bar></Bar>
      <Bar></Bar>
      <Bar></Bar>
    </div>
  );
}

export default Chart;

.bar {
  border-radius: 5px 5px 0 0;
  background-color: #ff4136;
  grid-row-start: 1;
  grid-row-end: 101;
}

import classes from "./Bar.module.css";

function Chart() {
  return <div className={classes.bar}></div>;
}

export default Chart;


