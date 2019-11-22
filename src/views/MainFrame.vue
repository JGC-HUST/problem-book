<template>
  <el-container>
    <el-header>
      <MainFrameHeader />
    </el-header>
    <el-container>
      <el-aside width="200px">
        <MainFrameAside />
      </el-aside>
      <el-main>
        <router-view />
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
import MainFrameAside from "../components/MainFrameAside";
import MainFrameHeader from "../components/MainFrameHeader";
export default {
  components: {
    MainFrameAside,
    MainFrameHeader
  }
};
</script>