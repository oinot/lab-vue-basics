<template class="get-posts">
  <div v-for="post in posts" :key="post.id">
    <h1>{{ post.title }}</h1>
    <p>{{ post.description }}</p>
    <p>{{ post.content }}</p>
  </div>
</template>

<script>

export default {
  name: 'getPosts',
  data() {
    return {
      posts: [
        {
          id: 0,
          title: 'Venenatis',
          description: 'Erat velit scelerisque in dictum non consectetur a erat. ',
          content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Magna fringilla urna porttitor rhoncus dolor purus non enim. Netus et malesuada fames ac turpis egestas maecenas pharetra. A iaculis at erat pellentesque adipiscing commodo elit at. Sed vulputate odio ut enim blandit volutpat maecenas volutpat. Lacus sed turpis tincidunt id aliquet. Sit amet tellus cras adipiscing enim eu turpis egestas pretium. Est lorem ipsum dolor sit amet consectetur adipiscing. Nisl rhoncus mattis rhoncus urna neque viverra justo. At auctor urna nunc id cursus metus. Malesuada fames ac turpis egestas sed tempus urna et pharetra. Risus commodo viverra maecenas accumsan lacus vel facilisis volutpat est. Aenean euismod elementum nisi quis eleifend quam adipiscing. Viverra vitae congue eu consequat ac felis donec.',
        },
        {
          id: 1,
          title: 'Etiam',
          description: 'Pharetra et ultrices neque ornare aenean euismod elementum nisi.',
          content: 'Venenatis urna cursus eget nunc scelerisque viverra mauris in aliquam. Aliquam sem fringilla ut morbi tincidunt augue interdum. Vitae purus faucibus ornare suspendisse sed nisi. Id semper risus in hendrerit gravida rutrum quisque non tellus. Ac auctor augue mauris augue. In hendrerit gravida rutrum quisque non tellus orci ac. Ac turpis egestas sed tempus. Mattis aliquam faucibus purus in. Morbi tempus iaculis urna id. Quam elementum pulvinar etiam non quam lacus suspendisse. Nunc eget lorem dolor sed viverra ipsum nunc aliquet.',
        },
        {
          id: 2,
          title: 'Sed',
          description: 'Etiam erat velit scelerisque in dictum non consectetur',
          content: 'Sed vulputate mi sit amet. In est ante in nibh mauris cursus mattis. Dictum fusce ut placerat orci nulla pellentesque. Sagittis eu volutpat odio facilisis mauris sit amet massa. Id leo in vitae turpis massa sed elementum tempus. Tellus id interdum velit laoreet id donec ultrices tincidunt. Viverra nam libero justo laoreet sit amet. Sit amet consectetur adipiscing elit pellentesque habitant morbi tristique. Nibh ipsum consequat nisl vel pretium lectus quam. Id eu nisl nunc mi ipsum faucibus. Eu turpis egestas pretium aenean pharetra. Eu turpis egestas pretium aenean pharetra.',
        },
      ],
    };
  },
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

div {
  display: flex;
  flex-direction: column;
  justify-content: left;
  padding: 30px;
  text-align: left;
}

p, h1 {
  list-style-type: none;
  margin: 10px 0 0 0;
  color: white;
}
</style>
