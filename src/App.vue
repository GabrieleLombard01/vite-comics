<script>
import appHeader from './components/appHeader.vue';
import appJumbo from './components/appJumbo.vue';
import appCategory from './components/appCategory.vue';
import appFooter from './components/appFooter.vue';
export default {
  data() {
    return {

    }
  },
  components: { appHeader, appJumbo, appCategory, appFooter }
}
</script>

<template>
  <!--HEADER-->
  <appHeader />

  <!--MAIN-CONTENT-->
  <main>

    <!--JUMBO-->
    <appJumbo />

    <!--CATEGORY-->
    <appCategory />

    <!--FOOTER-->
    <appFooter />

  </main>
</template>

<style >
main {
  background-color: rgb(215, 215, 215);
  width: 100%;
  color: white;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
  color: white;
}

.container {
  width: 1200px;
  margin: 0 auto;
  border: dashed white 1px;
}

.small_size {
  width: 50px;
}
</style>
