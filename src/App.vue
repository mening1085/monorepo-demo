<script setup>
import { ref } from "vue";
import TextInput from "./components/TextInput.vue";

const msg = ref("Hello Vue 3 + Vite");
</script>

<template>
  <div>
    <h1 class="text-3xl font-bold underline mb-12">Hello Monorepo!</h1>
    <text-input :value="msg" @event:update="msg = $event" />

    <div class="mt-12">
      {{ msg }}
    </div>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
