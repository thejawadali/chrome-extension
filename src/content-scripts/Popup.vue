<script setup>
import { ref } from "vue"

const visible = ref( false )

</script>
<template>
  <div class="overlay" v-show="visible">
    <div class="popup">
      <h1>Hello, Vite-Plugin-Chrome-Extension</h1>
    </div>
  </div>
</template>

<style>
.overlay {
  @apply fixed inset-0 w-full h-full bg-black bg-opacity-10 z-50;
}

.popup {
  @apply absolute top-4 right-4 bg-white shadow-lg p-4 rounded-md w-72;
}
</style>
