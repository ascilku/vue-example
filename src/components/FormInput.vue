<script setup>
defineProps({
  name: {
    type: String,
    required: true,
  },
});

</script>

<template>
  <div>
    <label for="name" class="label">Name {{ name }}</label>
    <input
      id="name"
      type="text"
      class="input"
      placeholder="Enter your name"
      v-model="test"
    />
    <p>ini test {{ test }}</p>
  </div>
</template>

<script>

export default {
  data() {
    return {
      test: "",
    };
  },
};

</script>
