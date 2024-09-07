<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div style="width:100vw;height:100vh;">
  <HelloWorld msg="yaku.icu 建设中" />
    
</div>
</template>

<style scoped>
*{
margin:0px;
padding:0px;
border:0px;
}
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
