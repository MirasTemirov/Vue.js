<template>
  <header class="header">
    <h1 class="title">KBTU</h1>
    <nav class="nav">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Grade</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 20px 0;
  background-color: #333;
  color: white;
  width: 100%;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  position: sticky;
  top: 0;
  z-index: 1000;
  margin: 0;
}

.title {
  font-size: 2rem;
  margin: 0;
  text-align: center;
}

.nav {
  margin-top: 10px;
}

.nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  gap: 20px;
}

.nav ul li a {
  color: white;
  text-decoration: none;
  font-size: 1rem;
}

.nav ul li a:hover {
  text-decoration: underline;
}
</style>
