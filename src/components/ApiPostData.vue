<template>
  <div>
    <div class="header">
      <h1>Post Data From API Request</h1>
      <div v-for="(post, key) in postdata" :key="post.id">
        <h3>{{ key + 1 }}---- {{ post.title }}</h3>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      postdata: [],
    };
  },
  created() {
    axios
      .get("https://jsonplaceholder.typicode.com/posts")
      .then((response) => {
        this.postdata = response.data;
      })
      .catch((error) => {
        console.log("You Error is - " + error);
      });
  },
};
</script>

<style scoped>
.header {
  width: 960px;
  margin: 10px auto;
  padding: 5px 10px;
}
</style>
