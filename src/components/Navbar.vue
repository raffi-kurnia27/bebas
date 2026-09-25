<template>
  <header class="navbar">
  <nav>
    <h2>SMK Yadika Soreang - Onlineshop</h2>
    <RouterLink to="/">Landing</RouterLink> |
    <RouterLink to="/product">Product</RouterLink> |
    <RouterLink to="/about">About</RouterLink>
    <RouterLink to="/contact">contact</RouterLink>
  </nav>

  </header>
</template>

<style scoped>

.navbar {
  max-width: 2000px;
  height: 75px;
  margin: auto;
  padding: 0 25px;

  display: flex;
  align-items: center;
  justify-content: space-between;

  background: whitesmoke;
}

.navbar h2 {
  margin: 0;
  color: black;
  font-size: 20px;
}

nav {
  display: flex;
  gap: 25px;
}

nav a {
  color: gray;
  text-decoration: none;
}

nav a:hover {
  color: darkblue;
}

nav a.router-link-active {
  color: darkblue;
  font-weight: bold;
}
</style>