<template>
  <div class="home">
    <changeBgColor />
    <tomorrowIs />
    <getPosts />
  </div>
</template>

<script>
import getPosts from '../components/posts.vue';
import tomorrowIs from '../components/math.vue';
import changeBgColor from '../components/changeColor.vue';

export default {
  name: 'HomeView',
  components: {
    tomorrowIs,
    getPosts,
    changeBgColor,
  },
};
</script>
