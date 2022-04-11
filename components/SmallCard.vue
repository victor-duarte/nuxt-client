<template>
  <NuxtLink :to="`/products/${card.id}`" class="card-container">
    <img :src="require(`@/assets/images/${card.image}`)" alt="" class="image" />
  </NuxtLink>
</template>

<script>
export default {
  props: ["card"],
};
</script>

<style scoped>
.card-container {
  border-radius: 0.5rem;
  cursor: pointer;
  height: 12.5rem;
  margin-bottom: 1.5rem;
  overflow: hidden;
  width: 24%;
}

.image {
  height: 100%;
  width: 100%;
}
</style>
