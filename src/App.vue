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
  <div class="container-wrapper">
    <!--HEADER-->
    <appHeader />

    <!--MAIN-CONTENT-->
    <main class="main-content">

      <!--JUMBO-->
      <appJumbo />

      <!--CATEGORY-->
      <appCategory />

    </main>


    <!--FOOTER-->
    <appFooter />
  </div>
</template>

<style >
.container-wrapper {
  display: flex;
  flex-direction: column;
}

.main-content {
  flex-grow: 1;
  z-index: 1;
}

main {
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
