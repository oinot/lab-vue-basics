<template>
  <footer>
  <h1> {{ msg }}</h1>
  <div class="parent">
    <div class="div1">Every </div>
    <div class="div2">Day </div>
    <div class="div3">Is like </div>
    <div class="div4">Monday </div>
  </div>
  </footer>
</template>

<script>
export default {
  name: 'footerComponent',
  data() {
    return {
      msg: 'This is a Footer',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

footer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.parent {
  display: grid;
  width: 200px;
  height: 100px;
  text-align: center;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  grid-column-gap: 5px;
  grid-row-gap: 5px;
}

.div1 { grid-area: 1 / 1 / 2 / 2; }
.div2 { grid-area: 1 / 2 / 2 / 3; }
.div3 { grid-area: 2 / 1 / 3 / 2; }
.div4 { grid-area: 2 / 2 / 3 / 3; }

* {
  color: aliceblue;
}

</style>
