<template>
  <HeaderC />
  <MainComponent />
  <FooterComponent />
</template>

<script>
import HeaderC from './components/HeaderC.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderC,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;600&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Passion+One&display=swap');
</style>

