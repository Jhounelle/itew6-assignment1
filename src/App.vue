<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/skills">Skills</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style>
  header {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    background-color: #f8f9fa;
    padding: 1rem 0;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1000;
  }

  nav {
    display: flex;
    gap: 20px;
  }

  nav a {
    text-decoration: none;
    color: #333;
    font-size: 1.2rem;
    font-weight: bold;
    padding: 10px;
    transition: color 0.3s;
  }

  nav a:hover {
    color: #00ff62;
  }

  body {
    background-image: url("./assets/images/bg2.jpg");
    background-size: 100%;
    background-repeat: no-repeat;
    margin: 0;
    padding-top: 60px;
  }
</style>
