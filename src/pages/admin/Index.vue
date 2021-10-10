<template>
  <h1>Protected route</h1>
  <h3>Olá {{ getMe.username }}</h3>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Index',
  computed: {
    ...mapGetters('auth', ['getMe'])
  }
}
</script>

<style scoped>

</style>
