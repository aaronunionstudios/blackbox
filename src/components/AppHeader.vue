<script setup>
defineProps({
  msg: {
    type: String,
    // required: true
  }
})
</script>

<template>
  <div class="header flex-row">
    <div class="flex-child">AW</div>
     <div class="flex-child">{{ msg }}</div>
  </div>
</template>

<style scoped>
.header {
    width: 100%;
    background-color: black;
    color: whitesmoke;
    padding:10px;
}
</style>