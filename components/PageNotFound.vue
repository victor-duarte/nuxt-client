<template>
  <div>
    <h1>Page Not Found</h1>
    <img :src="require('@/assets/images/fe25.jpg')" alt="" />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
div {
  align-items: center;
  display: flex;
  justify-content: center;
  margin: 0 auto;
  width: 50%;
}

h1 {
  font-size: 7.5rem;
}

img {
  margin: 0 auto;
  width: 15rem;
}
</style>
