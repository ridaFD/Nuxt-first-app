<template>
  <div>
    <nuxt-child />
    <input v-model="userId" type="text">
    <button @click="onLoadUser">Load User</button>
  </div>
</template>

<script>
export default {
  name: "users",
  data() {
    return {
      userId: null
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId)
    }
  },
  layout: 'users'
}
</script>

<style scoped>

</style>