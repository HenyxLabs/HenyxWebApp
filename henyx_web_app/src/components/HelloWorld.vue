<script setup lang="ts">
</script>

<template>
  <div class="main">
    <div class="logo">
      <img src="/src/assets/LogoHenyx.png" alt="Company Logo">
    </div>
    <div class="navbar">
      <nav>
        <ul>
          <li><a class="hover-underline" href="#">Blog</a></li>
          <li><a class="hover-underline" href="#">Projects</a></li>
          <li><a class="hover-underline" href="#">Services</a></li>
          <li><a class="hover-underline" href="#">About us</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<style scoped>
.logo {
  width: 100vw;
  margin-top: 10vh;
  margin-bottom: 10vh;
}
.logo > img{
  width: 70vw;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.navbar{
  width: 100vw;
  margin-top: 10vh;
  margin-bottom: 10vh;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  text-align:center;
}

li {
  display: inline-block;
  margin-left: 1vw;
  margin-right: 1vw;
}

li > a {
  text-decoration: none;
  color: #00ff00;
  padding: 5px;
}

.hover-underline {
  font-size: 1rem;
  color: #00ff00;
  position: relative;
  display: inline-block;
}

.hover-underline::after,
.hover-underline::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 2px;
  background: linear-gradient(to right, #000000, #00ff00);
  bottom: -5px;
  left: 0;
  transform: scaleX(0);
  transform-origin: right;
  transition: transform 0.4s ease-out;
}

.hover-underline::before {
  top: -5px;
  transform-origin: left;
}

.hover-underline:hover::after,
.hover-underline:hover::before {
  transform: scaleX(1);
}
</style>
