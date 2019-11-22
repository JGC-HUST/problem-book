<template>
  <div>
    <el-row :gutter="20" style="margin-bottom: 20px">
      <el-col :span="6" v-for="(i, index) in cates" :key="index">
        <CateCard :title="i.title" :num="i.num" />
      </el-col>
    </el-row>

    <el-row :gutter="20">
      <el-col :span="6">
        <CateCard :title="'数量'" :num="0" />
      </el-col>
    </el-row>
  </div>
</template>

<script>
import CateCard from "@/components/CateCard";
export default {
  name: "home",
  components: {
    CateCard
  },
  data() {
    return {
      cates: [
        {
          title: "常识",
          num: 0
        },
        {
          title: "言语",
          num: 0
        },
        {
          title: "资料",
          num: 0
        },
        {
          title: "判断",
          num: 0
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>
