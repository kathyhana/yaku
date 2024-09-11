<script setup>
import { onMounted, ref } from 'vue'
/* import Lottie from '@lottielab/lottie-player/web' */

onMounted(() => {
console.log(VANTA)

VANTA.GLOBE({
  el: "#halo",
  mouseControls: true,
  touchControls: true,
  gyroControls: false,
  minHeight: 200.00,
  minWidth: 200.00,
  scale: 1.00,
  scaleMobile: 1.00,
  color: 0x2e2e16,
  backgroundColor: 0xe5e1ed
})
})

defineProps({
  msg: String,
})

const count = ref(0)

</script>


<template>
<div id="halo" style="width:100vw;height:100vh">

    <h1>{{ msg }}</h1>

</div>
</template>

<style scoped>
*{
margin:0px;
padding:0px;
border:0px;
}
.read-the-docs {
  color: #888;
}
</style>
