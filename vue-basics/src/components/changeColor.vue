<template>
  <button @click="toggleButton()">Change color</button>
  <div :class="[toggler ? 'one-bg-color' : 'another-bg-color']"></div>
</template>

<script>
export default {
  name: 'changeBgColor',
  data() {
    return {
      toggler: true,
    };
  },
  methods: {
    toggleButton() {
      this.toggler = !this.toggler;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.one-bg-color,
.another-bg-color {
  height: 100px;
  margin: 5px 30px;
}

.one-bg-color {
  background: rgb(88, 88, 104);
}

.another-bg-color {
  background: rgb(176, 176, 199);
}
button {
  padding: 10px 20px;
  margin: 30px;
  background: black;
  border: none;
  border-radius: 4px;
  color: beige;
  cursor: pointer;
}
</style>
