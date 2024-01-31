<template>
  <div>
    <input
      type="text"
      :value="value"
      class="border-2 border-gray-400 px-3 py-1 rounded-md min-h-[40px]"
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

<style></style>
