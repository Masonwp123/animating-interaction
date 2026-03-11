<script setup>
defineProps(['show'])
</script>

<template>
  <div class="flip-card">
    <div class="flip-card-inner" :class="{flipped: show}">
      <div class="flip-card-slot flipped">
        <slot name="front"/>
      </div>
      <div class="flip-card-slot">
        <slot name="back"/>
      </div>
    </div>
  </div>
</template>

<style scoped>
.flip-card {
  background-color: transparent;
  width: 300px;
  height: 200px;
  perspective: 1000px;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.8s;
  transform-style: preserve-3d;
}

.flipped {
  transform: rotateY(180deg);
}

.flip-card-slot {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}
</style>