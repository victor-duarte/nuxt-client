<template>
  <div class="container">
    <h4 class="header">{{ cardsSection.title }}</h4>
    <p class="snippet">{{ cardsSection.snippet }}</p>
    <div class="cards-container">
      <LargeCard
        :card="card"
        :key="card.id"
        v-for="card in cardsSection.cards"
      />
    </div>
  </div>
</template>

<script>
import LargeCard from "./LargeCard.vue";
export default {
  props: ["cardsSection"],
  components: { LargeCard },
};
</script>

<style scoped>
.container {
  margin-top: 2rem;
}

.header {
  font-size: 1.5rem;
  font-weight: 700;
}

.snippet {
  color: grey;
  margin-bottom: 1.5rem;
}

.cards-container {
  display: flex;
  justify-content: space-between;
}
</style>
