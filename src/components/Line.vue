<template lang="html">
  <div>
    <line-chart v-bind:height="350"></line-chart>
  </div>
</template>

<script>
import LineChart from '../charts/LineChart.js'

export default {
  components: {
    'line-chart': LineChart
  }
}
</script>

<style lang="css">
</style>
