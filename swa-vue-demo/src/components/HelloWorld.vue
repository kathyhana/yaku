<script setup>
import { onMounted, ref } from 'vue'
/* import Lottie from '@lottielab/lottie-player/web' */

onMounted(() => {
console.log(VANTA)

VANTA.DOTS({
  el: "#halo",
  mouseControls: true,
  touchControls: true,
  gyroControls: false,
  minHeight: 200.00,
  minWidth: 200.00,
  scale: 1.00,
  scaleMobile: 1.00,
  color: 0xb60b4a,
  color2: 0xffffff,
  backgroundColor: 0x151415,
  size: 6.10
})
})

defineProps({
  msg: String,
})

const count = ref(0)

  delay:        .4*DURATION,
  isShowStart:  true
});

const closeTimeline = new mojs.Timeline();
closeTimeline
  .add(
    closeX, closeCircle,
    fadeTimeline
);

openTimeline.replay();
circle.el.addEventListener( 'click', function () {
  circle._hide();
  openTimeline.stop();
  closeTimeline.replay();
  openBackground.replayBackward();
});

</script>


<template>
<div style="width:100vw;height:100vh">

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
body, html {
  padding: 0;
  margin:  0;
  width: 100%;
  height: 100%;
  overflow: hidden;
}

body {
  background: rgba(241, 226, 215, 0.2);
  position: relative;
  // background: #FC2D79;
  background: #28143F;
}

.close-button {
  cursor: pointer;
}
</style>
