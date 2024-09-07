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
  scaleMobile: 1.00
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
