<template>
    <div>
        <h2>{{msg}}</h2>
        <el-carousel :interval="2000" type="card" height="200px">
            <el-carousel-item v-for="item in 6" :key="item">
            </el-carousel-item>
        </el-carousel>
        <router-view></router-view>
    </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "脚手架测试"
    };
  }
};
</script>

<style scoped>
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 200px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>