<template>
<body>
  <headerComponent />
  <footerComponent />
</body>
</template>

<script>
import headerComponent from './components/header.vue';
import footerComponent from './components/footer.vue';

export default {
  components: {
    headerComponent,
    footerComponent,
  },
};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  border-radius: 4px;
}

body {
  width: 600px;
  height: auto;
  margin: 5vh auto;
  background-color: #130f0f8f;
  border-radius: 6px;
}

</style>
