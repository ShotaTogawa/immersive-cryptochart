<template>
  <div id='board'>
    {{ label }}
    {{ value }}
  </div>
</template>

<script>
export default {
  name: 'Metric',
  props:
    [
      'label',
      'currentValue',
      'changeInTheDay',
      'highestValue',
      'lowestValue',
      'volume',
      'marketCap',
    ],
};
</script>

<style>
div#board{
  background-color: lightgray;
  width: 120px;
  height: 60px;
  text-align: center;
  margin: 0 auto;
  float: left;
  margin-left: 20px;
}
</style>

