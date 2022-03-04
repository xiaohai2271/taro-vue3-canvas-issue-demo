<template>
  <view class="index">
    <canvas
      type="2d"
      class="canvas-demo"
      :disableScroll="true"
      @onTouchStart="onTouchStart"
      @onTouchMove="onTouchMove"
      @onTouchEnd="onTouchEnd"
      @onTouchCancel="onTouchCancel"
      @onLongTap="onLongTap"
      @onError="onError"
    >
    </canvas>
  </view>
</template>

<script>

export default {
  name: 'Index',
  methods: {
    onTouchStart(e) {
      console.log('onTouchStart', e)
    },
    onTouchMove(e) {
      console.log('onTouchMove', e)
    },
    onTouchEnd(e) {
      console.log('onTouchEnd', e)
    },
    onTouchCancel(e) {
      console.log('onTouchCancel', e)
    },
    onLongTap(e) {
      console.log('onLongTap', e)
    },
    onError(e) {
      console.log('onError', e)
    },
  }
}
</script>

<style>
.index {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
