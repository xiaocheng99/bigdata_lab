<template>
  <div class="homeBody">
    <div class="header">
      <el-carousel :interval="5000" arrow="always" class="slider_container" height="100%" >
        <el-carousel-item v-for="item in 4" :key="item" >
          <h3>ssss</h3>
        </el-carousel-item>
      </el-carousel>
    </div>
   
  </div>

</template>





  <script>

    export default {
      name: 'HomeView',
      data() {
        return {
          activeIndex: '1',
          activeIndex2: '1'
        };
      },
      methods: {
        handleSelect(key, keyPath) {
          console.log(key, keyPath);
        }
      }
    }
  
  </script>
  
<style scoped>
@import url(../assets/css/HomeView.css);
</style>