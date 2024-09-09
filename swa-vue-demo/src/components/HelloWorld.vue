<script setup>
import { onMounted, ref } from 'vue'
/* import Lottie from '@lottielab/lottie-player/web' */



onMounted(() => {
console.log(VANTA)
VANTA.bird({
  el: "#bird",
  mouseControls: true,
  touchControls: true,
  gyroControls: false,
  minHeight: 200.00,
  minWidth: 200.00,
  baseColor: 0xffffff,
  backgroundColor: 0x0,
  amplitudeFactor: 0.30,
  xOffset: -0.06,
  yOffset: -0.10,
  size: 0.50


const player = new Lottie();
document.getElementById("bird").appendChild(player);

  player.setAttribute("src", "https://cdn.lottielab.com/l/7UjyCk4NGXBHkg.html");
player.play();

}
         )

defineProps({
  msg: String,
})

const count = ref(0)



</script>


<template>
<div id="bird" style="width:100vw;height:100vh">

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
