<template>
  <section class="container">
    <Header />
    <nuxt-link to="/users">Users</nuxt-link>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'
import Header from "~/components/Header.vue";

export default Vue.extend({
  components: {Header}
})
</script>

<style>

</style>
