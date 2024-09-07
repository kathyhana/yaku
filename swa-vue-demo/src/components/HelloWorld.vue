<script setup>
import { onMounted, ref } from 'vue'

onMounted(() => {
console.log(VANTA)
VANTA.BIRDS({
  el: "#bird",
  mouseControls: true,
  touchControls: true,
  gyroControls: false,
  minHeight: 200.00,
  minWidth: 200.00,
  scale: 1.00,
  scaleMobile: 1.00,
  backgroundColor: 0xfdfdfd,
  color1: 0x0,
  color2: 0x8f8f8f,
  colorMode: "lerpGradient",
  birdSize: 1.30,
  wingSpan: 37.00,
  speedLimit: 10.00,
  separation: 100.00,
  alignment: 84.00,
  cohesion: 64.00,
  quantity: 3.00
})

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
