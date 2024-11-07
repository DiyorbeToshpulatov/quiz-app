<template>
  <div class="results">
    <p>Your Results...</p>
    <h1>{{ numberOfCorrectAnswers }} / {{ quizQuestionLength }}</h1>
    <button class="btn" @click="router.push('/')">Go Home</button>
  </div>
</template>

<script setup>
import { useRouter } from "vue-router";

const router = useRouter();

const { numberOfCorrectAnswers, quizQuestionLength } = defineProps([
  "quizQuestionLength",
  "numberOfCorrectAnswers",
]);
</script>

<style scoped>
.results {
  text-align: center;
  padding: 100px 0;
}

p {
  font-size: 25px;
}

h1 {
  font-size: 80px;
}

.btn {
  background-color: darkblue;
  color: white;
  padding: 10px 40px 10px 40px;
  font-size: 20px;
  cursor: pointer;
  border-radius: 10px;
}
</style>
