<template>
  <img id="heartbeat" src="../assets/heart-full-red.svg" style="width:16px !important; height:16px !important; margin-right:5px; margin-bottom:-2px;">
</template>

<script>
export default {
  data() {
    return {}
  }
}
</script>

<style scoped>

#heartbeat {
  /*pointer-events: visible;*/
  animation: pulsateSmaller 1s;
  animation-iteration-count: infinite;
  width: 20px;
  height: 20px;
}

@keyframes pulsateSmaller {
    0% {
        transform: scale(1.0,1.0)
    }

    50% {
        transform: scale(0.8,0.8)
    }

    100% {
        transform: scale(1.0,1.0)
    }
}
</style>
