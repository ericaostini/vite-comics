<template>
  <div>
    <HeaderC />
    <MainComponent />
    <footer>Footer</footer>
  </div>
</template>

<script>
import HeaderC from './components/HeaderC.vue';
import MainComponent from './components/MainComponent.vue';
export default {
  name: 'App',
  component: {
    HeaderC,
    MainComponent
  }
}
</script>

<style lang="scss" scoped></style>
