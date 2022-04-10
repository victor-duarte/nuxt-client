<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark padding">
    <a class="navbar-brand" href="/">Firengii</a>
    <button
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
      class="navbar-toggler"
      data-target="#navbarSupportedContent"
      data-toggle="collapse"
      type="button"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse ml-auto" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item active">
          <a href="/products" class="nav-link">
            Products <span class="sr-only">(current)</span>
          </a>
        </li>
        <li class="nav-item active">
          <a href="/my-items" class="nav-link">
            My Items <span class="sr-only">(current)</span>
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
.padding {
  background-color: black;
  padding: 1.5rem;
}

.nav-left {
  margin-left: auto;
}
</style>
