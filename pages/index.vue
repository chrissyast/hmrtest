<template>
  <my-component />
</template>

<script>
export default {
  components: {
    MyComponent: () => import("~/components/MyComponent.vue")
  },
  mounted() {
    console.log("in page")
    console.log(this.$nuxt.context.isHMR)
  }
  // make some changes
}
</script>
