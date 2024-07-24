<script>

export default {
  props: ["modelValue", "msg"],
  emits: ["update:modelValue"],
};
</script>

<template>
  <h1>{{ msg }}</h1>

  <br />

  <input :value="modelValue" @input="$emit('update:modelValue', $event.target.value)" />
</template>

<style scoped>
.read-the-docs {
  color: #888;
}

.horizontal {
  display: flex;
  justify-content: center;
  align-items: center;
  column-gap: 2rem;
}
</style>
