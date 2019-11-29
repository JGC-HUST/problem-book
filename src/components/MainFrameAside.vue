<template>
  <div id="container">
    <el-row>
      <el-col>
        <el-menu
          class="el-menu-vertical-demo"
          router
          @open="handleOpen"
          @close="handleClose"
          @select="handleOpen"
        >
          <el-menu-item index="/list">
            <span slot="title">常识</span>
          </el-menu-item>

          <el-submenu index="2">
            <template slot="title">
              <span>言语</span>
            </template>
            <el-menu-item index="2-1">片段阅读</el-menu-item>
            <el-menu-item index="2-2">语言运用</el-menu-item>
            <el-menu-item index="2-3">选词填空</el-menu-item>
          </el-submenu>

          <el-menu-item index="3">
            <span slot="title">资料</span>
          </el-menu-item>

          <el-submenu index="4">
            <template slot="title">
              <span>判断</span>
            </template>
            <el-menu-item index="4-1">图形推理</el-menu-item>
            <el-menu-item index="4-2">类比推理</el-menu-item>
            <el-menu-item index="4-3">定义判断</el-menu-item>
            <el-menu-item index="4-4">逻辑推理</el-menu-item>
          </el-submenu>

          <el-submenu index="5">
            <template slot="title">
              <span>数量</span>
            </template>
            <el-menu-item index="5-1">数字推理</el-menu-item>
            <el-menu-item index="5-2">数量计算</el-menu-item>
          </el-submenu>
        </el-menu>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  methods: {
    handleOpen(index, indexPath) {
      console.log(index, indexPath);
    },
    handleClose(index, indexPath) {
      console.log(index, indexPath);
    }
  }
};
</script>

<style scoped>
#container {
  border-top: 1px solid #000;
}
</style>