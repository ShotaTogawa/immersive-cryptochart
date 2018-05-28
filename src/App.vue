<template>
  <div id="app">
    <Dashboard />
  </div>
</template>

<script>
import Dashboard from './components/Dashboard';
import Header from './components/Header';
import Content from './components/Content';
import Metric from './components/Metric';
import Footer from './components/Footer';
import Chart from './components/Chart';

export default {
  name: 'App',
  components: {
    Dashboard,
    Header,
    Content,
    Metric,
    Footer,
    Chart,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
