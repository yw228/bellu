<script>
export default {
  name: 'Header'
}
</script>

<template>
  <header>
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/hair-test">Hair Test</a></li>
        <li><a href="/how-it-works">How It Works</a></li>
        <li><a href="/bellu-university">Bellu University</a></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
header {
  background-color: #f5f5f5;
  padding: 1em 0;
}

nav ul {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
}

nav ul li {
  margin: 0 1em;
}

nav ul li a {
  text-decoration: none;
  color: #333;
}
</style>
