<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>

<div id="bird">
  <a href="https://www.baidu.com" target="_blank">
      <img src="./assets/yaku.jpg" class="logo vue" alt="yaku" />
    </a>
  </div>
  <HelloWorld msg="yaku.icu 建设中" />
</div>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r134/three.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/vanta@0.5.24/dist/vanta.birds.min.js"></script>
<script>
VANTA.BIRDS({
  el: "#bird",
  mouseControls: true,
  touchControls: true,
  gyroControls: false,
  minHeight: 200.00,
  minWidth: 200.00,
  scale: 1.00,
  scaleMobile: 1.00
})



    
</template>

<style scoped>
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
