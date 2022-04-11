<template>
  <div v-if="product" class="container py-5">
    <div class="hero-container">
      <img
        :src="require(`@/assets/images/${product.image}`)"
        alt=""
        class="image"
      />
      <div class="info-box">
        <h1>{{ product.title }}</h1>
        <p class="snippet">{{ product.snippet }}</p>
      </div>
    </div>
    <div class="whats-included-container">
      <div class="included-container">
        <h6>Super Effective</h6>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
      <div class="included-container">
        <h6>Clean & Tidy</h6>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
      <div class="included-container">
        <h6>Cancel Anytime</h6>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
      <div class="included-container">
        <h6>Satisfaction Guaranteed</h6>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores,
          dolorem.
        </p>
      </div>
    </div>
    <div class="description-container">
      <p>{{ product.description }}</p>
    </div>
  </div>
  <div v-else class="container mt-5">
    <p>Product {{ $route.params.id }} not found.</p>
  </div>
</template>

<script>
export default {
  computed: {
    product() {
      return this.$store.getters.getProductById(this.$route.params.id);
    },
  },
};
</script>

<style scoped>
.hero-container {
  display: flex;
  justify-content: space-between;
}

.image {
  height: 25rem;
  width: 59%;
}

.info-box {
  background-color: rgba(207, 201, 201, 0.322);
  border-radius: 0.5rem;
  padding: 1rem;
  width: 39%;
}

.whats-included-container {
  border-bottom: 0.1rem solid rgba(128, 128, 128, 0.151);
}

.description-container {
  border-bottom: 0.1rem solid rgba(128, 128, 128, 0.151);
  margin-bottom: 2rem;
  padding-bottom: 2rem;
}

.included-container {
  margin-top: 1.5rem;
}

h1 {
  font-size: 1.75rem;
}

h6 {
  font-size: 1.15rem;
  font-weight: 400;
}

p {
  color: grey;
}

.snippet {
  color: rgba(0, 0, 0, 0.774);
  margin-top: 1rem;
}

button {
  background-color: rgb(231, 81, 43);
  border-radius: 100rem;
  border: none;
  color: white;
  color: white;
  font-weight: 700;
  font-weight: 700;
  padding: 0.5rem;
  padding: 1rem 4rem;
  transition: 0.5s;
  width: 100%;
}

.description-container {
  color: grey;
  margin-top: 3rem;
}
</style>
