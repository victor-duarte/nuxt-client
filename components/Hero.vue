<template>
  <div class="Hero container">
    <div class="text-container">
      <h1 class="header">Find your Fire Extinguisher</h1>
      <p class="snippet">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iste iusto
        illum quidem asperiores, cum nisi aperiam eius ipsa sapiente odit!
      </p>
      <button class="button btn">Start Looking</button>
    </div>
    <img alt="" class="image" src="~assets/svg/fire-extinguisher.svg" />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.Hero {
  align-items: flex-start;
  display: flex;
  justify-content: space-between;
  padding: 5rem 0;
  position: relative;
}

.text-container {
  margin-top: 4rem;
  width: 50%;
}

.header {
  font-size: 5rem;
  font-weight: 900;
}

.snippet {
  color: grey;
  font-size: 1.25rem;
}

.image {
  margin-top: 2rem;
  width: 27.5rem;
}

.overlay {
  background: rgba(0, 0, 0, 0);
  height: 100%;
  position: absolute;
  top: 0;
  width: 100%;
}

.button {
  background-color: rgb(231, 81, 43);
  border-radius: 100rem;
  color: white;
  font-weight: 700;
  padding: 1rem 4rem;
  transition: 0.5s;
  width: 20rem;
}

.button:hover {
  width: 21.5rem;
}

@media (max-width: 500px) {
  .Hero {
    height: 40vh;
  }
}
</style>
