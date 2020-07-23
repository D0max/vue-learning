<template>
  <div>
    <component :is="layout">
      <router-view/>
    </component>
  </div>
</template>

<script>
  import Auth from '@/layouts/Auth'
  import MainLayout from '@/layouts/MainLayout'
  export default {
    computed: {
      layout() {
        console.log(this.$route.meta.layout)
        return 'empty-layout'
      }
    },
    components: {
      Auth, MainLayout
    }
  }
</script>

<style lang="scss">
  @import "~materialize-css/dist/css/materialize.min.css";
  @import "assets/index.css";
</style>
