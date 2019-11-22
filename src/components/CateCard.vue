<template>
  <el-card class="box-card">
    <div slot="header" class="clearfix card-head">
      <span class="card-title">{{ title }}</span>
      <el-button type="text" class="card-btn">查看</el-button>
    </div>
    <div class="text item">
      <span class="card-num">{{ num }}&nbsp;</span>道
    </div>
  </el-card>
</template>

<script>
export default {
  props: {
    num: {
      type: Number,
      default: 0
    },
    title: {
      type: String,
      default: "加载中"
    }
  },
  data() {
    return {};
  }
};
</script>

<style scoped>
.card-head {
  display: flex;
  align-items: baseline;
  position: relative;
}
.card-title {
  font-size: 24px !important;
  display: inline-block;
}
.card-btn {
  position: absolute;
  right: 15px;
}
.card-num {
  font-size: 60px;
}
</style>