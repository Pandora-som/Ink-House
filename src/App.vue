<template>
  <!--<InkHeader></InkHeader>-->
  <InkHeader />
  <router-view/>
  <InkFooter />
</template>
<script>
import InkFooter from "./components/InkFooter.vue";
import InkHeader from "./components/InkHeader.vue";
export default {
  components: {
    InkHeader,
    InkFooter
  },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0;
  padding: 0;
}
@media screen and (width <= 376px) {
  .AppFooter {
    display: none;
  }
}
</style>
