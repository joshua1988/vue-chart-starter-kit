<template>
  <div id="app">
    <el-row type="flex" class="row-bg" justify="center">
      <el-radio v-model="radio" label="bar">Bar</el-radio>
      <el-radio v-model="radio" label="line">Line</el-radio>
      <el-radio v-model="radio" label="pie">Pie</el-radio>
      <el-radio v-model="radio" label="bubble">Bubble</el-radio>
    </el-row>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      radio: ''
    }
  },
  watch: {
    radio() {
      this.navigateChart(this.radio);
    }
  },
  methods: {
    navigateChart(url) {
      this.$router.push(url);
    }
  },
  created() {
    this.radio = 'bar';
    this.navigateChart('bar');
  }
}
</script>

<style>
.el-row {
  margin-bottom: 20px;
  &:last-child {
    margin-bottom: 0;
  }
}
.el-col {
  border-radius: 4px;
}
.bg-purple-dark {
  background: #99a9bf;
}
.bg-purple {
  background: #d3dce6;
}
.bg-purple-light {
  background: #e5e9f2;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}
.row-bg {
  padding: 10px 0;
  background-color: #f9fafc;
}
</style>
