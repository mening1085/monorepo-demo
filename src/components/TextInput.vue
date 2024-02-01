<template>
  <div>
    <input
      type="text"
      :value="value"
      class="border-2 border-gray-400 px-3 py-1 rounded-md min-h-[40px] w-full bg-blue-500"
      @input="$emit('event:update', $event.target.value)"
    />
  </div>
</template>

<script setup>
import { ref } from "vue";

const props = defineProps({
  value: String,
});
</script>

<style>
.text__input {
  border: 2px solid #e2e8f0;
  border-radius: 0.375rem;
  padding: 0.75rem 1rem;
  min-height: 2.5rem;
  width: 100%;
  font-size: 1rem;
  line-height: 1.5rem;
  color: #111827;
  background-color: #c71515;
  transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
}
</style>
