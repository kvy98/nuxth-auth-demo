<template>
  <button @click="login">Google signin</button>
</template>
<script>
export default {
  methods: {
    login() {
      this.$auth.loginWith('google', { params: { prompt: 'select_account' } })
    },
  },
}
</script>
