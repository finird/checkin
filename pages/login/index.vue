<template>
  <!-- <html class="h-full bg-white">
        <body class="h-full"> -->
  <div class="h-full">
    <LoginForm></LoginForm>
  </div>
</template>

<script>
import LoginForm from "./LoginForm.vue";

export default defineComponent({
  components: {
    LoginForm,
  },
});
</script>
