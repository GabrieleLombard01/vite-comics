<script>
import appHeader from './components/appHeader.vue';
export default {
  data() {
    return {

    }
  },
  components: { appHeader }
}
</script>

<template>
  <!--HEADER-->
  <appHeader />

  <!--MAIN-CONTENT-->
  <main></main>
</template>

<style >
main {
  background-color: black;
  width: 100%;
  height: calc(100% - 180px);
  margin-top: 100px;
}
</style>
