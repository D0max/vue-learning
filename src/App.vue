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
        return (this.$route.meta.layout || 'empty') + '-layout'
      }
    },
    components: {
      EmptyLayout: Auth,
      MainLayout,
    }
  }
</script>

<style>
  @import "~materialize-css/dist/css/materialize.min.css";
  @import "assets/index.css";
</style>
