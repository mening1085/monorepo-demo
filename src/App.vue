<script setup>
import { ref } from "vue";
import TextInput from "./components/TextInput.vue";

const msg = ref("Hello Vue 3 + Vite");
</script>

<template>
  <div>
    <div
      class="p-12 border shadow-md rounded-2xl text-start min-w-[500px] flex justify-center flex-col"
    >
      <div class="mb-6">
        <div>Username</div>
        <text-input :value="msg" @event:update="msg = $event" />
      </div>
      <div>Password</div>
      <text-input :value="msg" @event:update="msg = $event" />
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
