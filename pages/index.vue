<template>
  <div class="container">
    <Hero />
    <LargeCardDisplay
      :cardsSection="cardInfo"
      :key="cardInfo.id"
      v-for="cardInfo in largeCardInfo"
    />
    <SmallCardDisplay
      :cardsSection="cardInfo"
      :key="cardInfo.id"
      v-for="cardInfo in smallCardInfo"
    />
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from "@/assets/data.js";

export default {
  name: "IndexPage",
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections,
    };
  },
};
</script>
