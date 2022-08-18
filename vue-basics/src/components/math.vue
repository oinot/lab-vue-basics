<template>
  <div class="tommorrow-is">
    <h1> Today's date is:</h1>
    <h2>{{ date }}</h2>
    <p v-if="isTrue = true">This is true:</p>
    <h3> if today is the {{ today }}, <br> tomorrow will be the {{ tomorrow }}</h3>
    <p>{{ printSomething() }}</p>

  </div>
</template>

<script>
export default {
  name: 'tomorrowIs',
  props: {
  },
  data() {
    return {
      date: new Date(),
      today: new Date().getDate([0]),
      tomorrow: new Date().getDate([0]) + 1,
      isTrue: true,
    };
  },
  methods: {
    printSomething() {
      return 'without a doubt';
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 10px 0 0;
}
.tommorrow-is {
  color: aliceblue;
  min-height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

</style>
