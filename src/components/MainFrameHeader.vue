<template>
  <div id="head">
    <div id="icon">行测笔记本</div>
    <div id="user">
      <el-popover placement="bottom" width="60" trigger="hover" id="pop">
        <template>
          <el-row class="cols">
            <el-button>个人资料</el-button>
          </el-row>
          <el-row class="cols">
            <el-button>退出系统</el-button>
          </el-row>
        </template>
        <span slot="reference">USER</span>
      </el-popover>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#head {
  display: flex;
  align-items: center;
  /* background-color: aqua; */
  height: 100%;
  width: 100%;
  border-bottom: 1px solid #000;
}
#head * {
  height: 20px;
  line-height: 20px;
}
#pop {
  width: 50px;
}
#pop:hover {
  cursor: pointer;
}
.cols * {
  width: 150px;
  border: none;
}
#user {
  position: absolute;
  right: 100px;
}
#icon {
  position: absolute;
  left: 50px;
  font-size: 30px;
}
</style>