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

<style lang="scss" scoped></style>
