<template lang="html">
  <div>
    <bar-chart v-bind:height="350"></bar-chart>
  </div>
</template>

<script>
import BarChart from '../charts/BarChart.js'

export default {
  components: {
    'bar-chart': BarChart
  }
}
</script>

<style lang="css">
</style>
