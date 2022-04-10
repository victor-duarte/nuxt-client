<template>
  <div class="card">
    <img :src="require(`@/assets/images/${card.image}`)" alt="" class="image" />
    <h3 class="header">{{ card.title }}</h3>
    <p class="snippet">{{ card.snippet }}</p>
  </div>
</template>

<script>
export default {
  props: ["card"],
};
</script>

<style scoped>
.card {
  border: none;
  cursor: pointer;
  height: 25rem;
  overflow: hidden;
  padding: 0;
  width: 31.5%;
}

.image {
  border-radius: 0.5rem;
  height: 65%;
}

.header {
  font-size: 1.15rem;
  margin-top: 0.4rem;
}

.snippet {
  color: grey;
}
</style>
