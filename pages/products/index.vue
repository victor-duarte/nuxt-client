<template>
  <div class="container">
    <LargeCardDisplay
      :cardsSection="cardInfo"
      :key="cardInfo.id"
      v-for="cardInfo in largeCardInfo.slice(0, 1)"
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
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections,
    };
  },
};
</script>

<style scoped></style>
