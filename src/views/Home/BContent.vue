<template>
  <div id="background"/>
  <a-flex id="title-group" justify="center" align="center" vertical="vertical">
    <div class="title">
      <span class="title">插件 </span><span class="title colored">下载中心</span>
    </div>
    <div class="info">
      登录你的账户查看所有你购买的插件，并且可以自由的下载使用它。<br>
      无需担心插件被删除，因为我们会一直保存你的插件。
    </div>
    <div class="button">
      <a-space>
        <a-button size="large" type="primary">进入管理平台</a-button>
        <a-button size="large" @click="joinQQTeam">加入交流群</a-button>
      </a-space>
    </div>
  </a-flex>
</template>

<script setup lang="ts">

import {qqTeam} from "@/api/text";

function joinQQTeam(){
  window.open(qqTeam)
}

</script>

<style scoped>
#background{
  position: absolute;
  background-image: url('@/assets/img/polygon-bg-element.svg');
  background-size: cover;
  background-position: center;
  height: 300px;
  width: 100%;
  z-index: 0;
}

#title-group{
  z-index: 20;
}

.title{
  font-size: 50px;
  font-weight: bold;
  transform: translateY(10vh);
}
.colored{
  background-image: linear-gradient(135deg,#1fa2ff,#12d8fa,#a6ffcb);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
  -webkit-text-fill-color: transparent;
}

.info{
  font-size: 20px;
  transform: translateY(15vh);
  width: 50%;
  text-align: center;
  color: #8c8c8c;
}
.button{
  transform: translateY(20vh);
}
</style>
