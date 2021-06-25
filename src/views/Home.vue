<template>
  <div class="home">
    <PostList :posts="posts" />
  </div>
</template>

<script>
import PostList from "../components/PostList.vue";
import { ref } from "@vue/reactivity";
export default {
  name: "Home",
  components: { PostList },
  setup() {
    const posts = ref([
      {
        title: "Windows 11 Released in 2021",
        body:
          "lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum ",
      },
      {
        title: "How to use Composition API in Vue 3",
        body:
          "lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum ",
      },
    ]);
    return { posts };
  },
};
</script>
