<template>
  <div>
    profile page for the user {{ $route.params.id }}
  </div>
</template>

<script>
export default {
  name: "index",
  validate(data) {
    console.log(data)
    // load the page if the id is number otherwise not
    return /^\d+$/.test(data.params.id)
  }
}
</script>

<style scoped>

</style>