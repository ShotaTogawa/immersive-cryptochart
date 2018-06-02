<template>
  <div id='container'>
      <Metric
       label='1 BTC <> JPY'
       v-bind:value ='currentValue'
       />
       <Metric
       label='24 Hour Change'
       v-bind:value ='changeInTheDay'
       />
       <Metric
       label='24 Hour High'
       v-bind:value ='highestValue'
       />
       <Metric
       label='24 Hour Low'
       v-bind:value ='lowestValue'
       />
       <Metric
       label='24 Hour Volume'
       v-bind:value ='volume'
       />
       <Metric
       label='Market Cap'
       v-bind:value ='marketCap'
       />
  
  </div>
</template>

<script>
import Metric from './Metric';
import Chart from './Chart';

export default {
  name: 'Content',
  components: {
    Metric,
    Chart,
  },
  data: () => {
    return {
      currentValue: 100000000,
      changeInTheDay: -190000,
      highestValue: 878000,
      lowestValue: 830000,
      volume: 540000,
      marketCap: 1391,
    };
  },
};
</script>

<style scoped>
  .metrics-container {
    display: flex;
    justify-content: center;
  }
</style>
