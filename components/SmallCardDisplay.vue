<template>
  <div class="container">
    <h4 class="header">{{ cardsSection.title }}</h4>
    <div class="card-container"></div>
  </div>
</template>

<script>
export default {
  props: ["cardsSection"],
};
</script>

<style scoped>
.container {
  padding: 2rem 0;
}

.header {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 2rem;
}

.card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
</style>
