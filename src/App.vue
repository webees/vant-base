<template>
  <div>
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App',
  watch: {
    $route() {
      window.document.title = this.$t(this.$route.meta.title)
    }
  }
}
</script>

<style lang="less" scoped></style>
