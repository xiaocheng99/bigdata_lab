<template>
  <div class="homeBody">
    <div class="header">
      <div class="navigate">
            <div class="navMenu">
              <div class="line"></div>
                      <el-menu 
                          :default-active="activeIndex2"
                          class="el-menu-navigate"
                          mode="horizontal"
                          @select="handleSelect"
                          text-color="#fff"
                          active-text-color="#ffd04b"
                          style="background: linear-gradient(rgb(17, 144, 203),rgb(124, 121, 121));
                                height:100%;
                                border-style: none;
                                padding-top: 2vw;
                                display:flex;
                                flex-direction:row;
                                
                                
                          "
                          >
                          
                          
                          <img src="http://bigdata.ahu.edu.cn/img/logo.png"  class="navMenu_logo">

                          <el-menu-item class="navMenu_tittle" index="1" style="font-size: 1.7vw;
                          margin-left:1.5vw;   
                          ">
                          首页
                          </el-menu-item>
                          <el-menu-item class="navMenu_tittle" index="2" style="font-size: 1.7vw;
                                ">
                          实验室介绍
                          </el-menu-item>
                          <el-menu-item class="navMenu_tittle" index="3"
                          style="font-size: 1.7vw;
                                "
                          >研发平台
                          </el-menu-item>
                          <el-menu-item class="navMenu_tittle" index="4" style="font-size: 1.7vw;
                                "
                          >学术成果
                          </el-menu-item>
                          <el-menu-item class="navMenu_tittle" index="5" 
                          style="font-size: 1.7vw;
                                "
                          >新闻公告
                          </el-menu-item>
                          <el-menu-item class="navMenu_tittle" index="6" style="font-size: 1.7vw;
                               "
                          >党团工作
                          </el-menu-item>
                          <el-menu-item class="navMenu_tittle" index="7" style="font-size: 1.7vw;
                                "
                          >友情链接
                          </el-menu-item>
                          <el-menu-item class="navMenu_tittle" index="8" style="font-size: 1.7vw;
                                "
                          >联系我们
                          </el-menu-item>
                          
                      </el-menu>
              </div>
          </div>     
          
      <el-carousel :interval="5000" arrow="always" class="slider_container" height="100%" >
      
        <el-carousel-item v-for="item in 4" :key="item" >
          
        </el-carousel-item>
      </el-carousel>
    </div>

  <div class="main">
      <div class="lab_infromation_container">
        <div class="lab_infromation lab_infromation_left">
          <div class="title_container">
              <p>实验室简介</p>
          </div>
          <div class="introduction_container">
            <div>
              　　安徽大学大数据与云服务工程实验室致力于数据管理与数据集成、海量知识库搭建与推理、机器学习与数据挖掘、数据流与复杂事件处理技术的研究及其在科学与工程领域中的应用。除此之外，实验室还注重实际应用的研究和实际问题的解决，在大数据研究和应用方面，采用Hadoop、Spark、Hive、Pig等云计算大数据平台。
            </div>
            
            <div>
               　　安徽大学大数据与云服务工程实验室致力于数据管理与数据集成、海量知识库搭建与推理、机器学习与数据挖掘、数据流与复杂事件处理技术的研究及其在科学与工程领域中的应用。除此之外，实验室还注重实际应用的研究和实际问题的解决，在大数据研究和应用方面，采用Hadoop、Spark、Hive、Pig等云计算大数据平台。
            </div>

            <div>
              　　实验室将秉承“博观约取，厚积薄发”的宗旨，贯彻“开放，合作，竞争”的方针，营造团队合作精神，积极进取，努力创新，将实验室打造为目标明确，富有干劲，能很好适应计算机新技术发展的科研队伍。在进行学术研究的同时，更加重视人才的培养，致力于培养具有研究能力、创新能力、开发能力、团队合作能力的跨领域人才，努力促进学科的可持续发展。
            </div>
          </div>
        </div>
        <div class="lab_infromation lab_infromation_right">
          <div class="img">
            
          </div>
          <div class="left">
            <div class="img">
            
            </div>
          </div> 
          <div class="right">
            
          </div>          
        </div>
      </div>


    <div class="lab_hardware_container">
      <div class="info_cricle info_cricle_index_1 ">

      </div>

      <div class="info_cricle info_cricle_index_2 ">
        
      </div>

      <div class="info_cricle info_cricle_index_3 ">
        
      </div>

      <div class="bottom_rec">
        
      </div>
    </div>

    <div class="lab_since_reserch_container">
      <div class="title_container">
        <p>科学研究</p>
      </div>

      <div class="info_reserch_container">
        <div class="info_reserch info_reserch_index_1">
          <div class="info_left">
            
          </div>
          <div class="info_right">
              <p class="tittle">超高性能、高精度算法研究平台</p>
              <p class="info">实验室为了提高效率，配置强劲的硬件，几十台高配置服务器组成的集群提供了强大的运算处理能力。</p>
          </div>
        </div>
        <div class="info_reserch info_reserch_index_2">
          
        </div>
        <div class="info_reserch info_reserch_index_3">
          
        </div>   
        <div class="info_reserch info_reserch_index_4">
          <div class="info_left">
            
          </div>

          <div class="info_right">
            
          </div>
        </div>
         
      </div>

    </div>

  <div class="more_info_container">
    
  </div>

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
          
        }
      }
    }
  
  </script>
  
<style scoped>
@import url(../assets/css/HomeView.css);
</style>