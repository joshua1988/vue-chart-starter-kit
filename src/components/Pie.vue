<template lang="html">
  <div class="">
    <pie-chart v-bind:height="350"></pie-chart>
  </div>
</template>

<script>
import PieChart from '../charts/PieChart.js'

export default {
  components: {
    'pie-chart': PieChart
  }
}
</script>

<style lang="css">
</style>
