<template>
  <div class="content">
    <h3> if today is {{ today }}, <br> tomorrow will be the {{ tomorrow }}</h3>
  </div>
</template>

<script>
export default {
  name: 'tomorrowIs',
  props: {
    msg: String,
  },
  data() {
    return {
      today: new Date().getDate([0]),
      tomorrow: new Date().getDate([0]) + 1,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 10px 0 0;
}
.content {
  color: aliceblue;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>
