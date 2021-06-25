<template>
  <h1>Post List</h1>
  <div v-for="post in posts" :key="post">
    <SinglePost :post="post" />
  </div>
</template>

<script>
import SinglePost from "../components/SinglePost.vue";
export default {
  props: ["posts"],
  components: { SinglePost },
};
</script>

<style></style>
