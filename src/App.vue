<script setup>
import QuizesView from "./views/QuizesView.vue";
</script>

<template>
  <div class="container">
    <RouterView />
    <!-- <QuizesView /> -->
  </div>
</template>

<style scoped>
.container {
  max-width: 1000px;
  margin: 0 auto;
}
</style>
