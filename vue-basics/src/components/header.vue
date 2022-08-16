<template>
    <nav>
    <router-link to="/">{{ home }}</router-link> |
    <router-link to="/about">{{ about }}</router-link>
  </nav>
  <router-view/>
</template>

<script>
export default {
  name: 'headerComponent',
  props: {
    msg: String,
  },
  data() {
    return {
      home: 'Home',
      about: 'About',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 10px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

nav {
  padding: 10px;
}

nav a {
  font-weight: bold;
  color: #9994b9;
}

nav a.router-link-exact-active {
  color: #d5d3e4;
}

</style>
