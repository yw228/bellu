<template>
  <nav class="navbar">
    <div class="navbar-brand">
      <img src="./pictures/img.png" alt="Bellu Logo"> <!-- Logo -->
    </div>
    <ul class="nav-tabs">
      <li class="nav-item"><router-link to="/" class="nav-link">Home</router-link></li>
      <li class="nav-item"><router-link to="/test" class="nav-link">Hair Test</router-link></li>
      <li class="nav-item"><router-link to="/work" class="nav-link">How Bellu Works</router-link></li>
      <li class="nav-item"><router-link to="/university" class="nav-link">Bellu University</router-link></li>
      <li class="nav-item"><router-link to="/about" class="nav-link">About Bellu</router-link></li>
    </ul>
    <div class="navbar-icons">
      <router-link to="/search">
        <img src="./icon/icons8-search-50.png" alt="Search" />
      </router-link> <!-- Search Icon -->
      <router-link to="/profile">
        <img src="./icon/icons8-person-64.png" alt="Search" />
      </router-link> <!-- People Icon -->
      <router-link to="/cart">
        <img src="./icon/icons8-shopping-bag-50.png" alt="Search" />
        </router-link> <!-- Shopping Bag Icon -->
    </div>
  </nav>
</template>

<script>

export default {
  name: 'NavBar'
}
</script>

<style>
.nav-tabs {
  display: flex;
  list-style: none;
  margin: 20px;
  padding: 0 10px;
  justify-content: space-between; /* This will space the tabs evenly */
}

.nav-item {
  /* Adjust padding if necessary, or add margin for additional spacing */
  padding: 0.5rem 1rem;
  margin: 0 10px; /* This will add space between each item */
}

.nav-link {
  text-decoration: none;
  color: grey; /* Change as needed */
  display: block;
  padding: 0.5rem 1rem;
  /* You can also add margin here if you need more control over the spacing */
}

.navbar {
  width: 100%; /* Full width */
  background-color: white;
  display: flex;
  justify-content: space-between; /* Spacing out logo and nav-items */
  align-items: center;
  padding: 0 10px; /* Padding on the sides */
}

.navbar-brand img {
  height: 50px; /* Adjust the logo size as needed */
}

.nav-menu li {
  padding: 14px 16px;
}

.nav-menu li a
.navbar-icons a{
  color: black;
  text-decoration: none;
}




</style>

