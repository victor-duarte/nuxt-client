<template>
  <div class="container">
    <Hero />
    <LargeCardDisplay
      :cardsSection="cardInfo"
      :key="cardInfo.id"
      v-for="cardInfo in largeCardInfo"
    />
  </div>
</template>

<script>
import { largeCardSections } from "@/assets/data.js";

export default {
  name: "IndexPage",
  data() {
    return {
      largeCardInfo: largeCardSections,
    };
  },
};
</script>
