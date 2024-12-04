<script setup>
defineProps({
  user: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div>
    <div>
      <h2>User info:</h2>
      <p>Name: {{ user.name }}</p>
      <p>Email: {{ user.email }}</p>
      <p>Password: {{ user.password }}</p>
      <p>Confirm Password: {{ user.passwordConfirmation }}</p>
    </div>
  </div>
</template>

<style scoped>
  p {
    font-family: Arial, sans-serif;
    margin: 5px 0;
  }
</style>
