<template>
  <div class="app">
    <Menu />

    <Main />
  </div>
</template>

<script>
import Menu from '@/components/Menu.vue'
import Main from '@/components/Main.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Main
  }
}
</script>

<style lang="scss">
@import '@/styles/global.scss';
</style>
