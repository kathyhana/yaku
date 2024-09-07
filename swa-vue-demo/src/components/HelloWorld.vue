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
  backgroundColor: 0xf0f0f0,
  color1: 0x0,
  color2: 0xef003b,
  birdSize: 1.60,
  wingSpan: 16.00,
  separation: 94.00,
  alignment: 88.00,
  cohesion: 25.00,
  backgroundAlpha: 0.57
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
.read-the-docs {
  color: #888;
}
</style>
