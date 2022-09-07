<template>
  <div class="the-card">
    <div class="the-card__title">{{ demo_title }}</div>
    <div class="the-card__body"><slot></slot></div>
  </div>
</template>

<script>
export default {
  props: {
    demo_title: {
      type: String,
    },
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
.the-card {
  width: 300px;
  min-height: 200px;
  border: 1px solid black;
  margin: 20px auto;
}
.the-card__title {
  background: rgb(2, 96, 2);
  padding: 5px 11px;
  color: #fff;
}
.the-card__body {
  padding: 11px;
}
.the-card__body img {
  height: 111px;
}
</style>
