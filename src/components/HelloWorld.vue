<script>
import { ref } from "vue";

export default {
  data() {
    return {
      message: "",
    };
  },

  mounted() {
    this.$refs.input.focus();

    console.log(this.$refs);
  },
};
</script>

<template>
  <p>Your message is: {{ message }}</p>
  <input ref="input" type="text" v-model="message" />
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
