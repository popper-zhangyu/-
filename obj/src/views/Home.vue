<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <keep-alive exclude="Home"> <input  -->
    <type="text" v-model="iptValue" v-if="isIptShow">
    <!-- </keep-alive> -->
   
    <button @click="isIptShow=!isIptShow">按钮</button>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data(){
    return{
      isIptShow:true,
      iptValue:""
    }
  }
}
</script>
