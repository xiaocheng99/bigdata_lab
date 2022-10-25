<template>


<div class="navigate">
  
    <div class="logo">
      <a href>
        <img >
      </a>
    </div>
    <div class="navMenu">
        <div class="line"></div>
        <el-menu 
            :default-active="activeIndex2"
            class="el-menu-demo"
            mode="horizontal"
            @select="handleSelect"
            background-color="#2d70c4"
            text-color="#fff"
            active-text-color="#ffd04b">
          
            <el-menu-item class="navMenu_tittle" index="1">首页</el-menu-item>
            <el-menu-item class="navMenu_tittle" index="2">实验室介绍</el-menu-item>
            <el-menu-item class="navMenu_tittle" index="3">研发平台</el-menu-item>
            <el-menu-item class="navMenu_tittle" index="4">学术成果</el-menu-item>
            <el-menu-item class="navMenu_tittle" index="5">新闻公告</el-menu-item>
            <el-menu-item class="navMenu_tittle" index="6">党团工作</el-menu-item>
            <el-menu-item class="navMenu_tittle" index="7">友情链接</el-menu-item>
            <el-menu-item class="navMenu_tittle" index="8">联系我们</el-menu-item>
        </el-menu>
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