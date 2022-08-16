<template>
  <div class="home">
    <tomorrowIs />
    <getPosts />
  </div>
</template>

<script>
import getPosts from '../components/posts.vue';
import tomorrowIs from '../components/math.vue';

export default {
  name: 'HomeView',
  components: {
    tomorrowIs,
    getPosts,
  },
};
</script>
