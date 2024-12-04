<script setup>
import FormSubmit from "@/components/FormSubmit.vue";
import FormDisplay from "@/components/FormDisplay.vue";

import { reactive } from "vue";

const userData = reactive({
  name: "",
  email: "",
  password: "",
  passwordConfirmation: "",
});

const handleFormSubmit = (userData) => {
  console.log("Реєстрація успішна. Ласкаво просимо, ", userData.name);
};
</script>

<template>
  <FormSubmit @submit="handleFormSubmit" user="userData" />
  <FormDisplay :user="userData" />
</template>

<style scoped></style>
