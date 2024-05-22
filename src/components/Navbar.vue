<template>
  <nav class="navbar">
    <div class="navbar-brand">
      <a class="navbar-item" href="#">
        Limbo 
      </a>
    </div>
    <div class="navbar-menu">
      <a class="navbar-item" href="#">Home</a>
      <a class="navbar-item" href="#">Shop</a>
      <a class="navbar-item" href="#">Contact</a>
    </div>
  </nav>
</template>



<script>
  export default {
    name: 'Navbar'
  };
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 30px;
  background-color: #333;
  color: white;
}
.navbar a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
  font-size: 20px;
}
.navbar a:hover {
  text-decoration: underline;
}
</style>