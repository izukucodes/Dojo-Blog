<template>
  <h1>{{ post.title }}</h1>
  <p>{{ snippet }}</p>
</template>

<script>
import { computed } from "@vue/runtime-core";
export default {
  props: ["post"],
  setup(props) {
    const snippet = computed(generateSnippet);

    function generateSnippet() {
      return props.post.body.substr(0, 100) + "...";
    }
    return { snippet };
  },
};
</script>

<style></style>
