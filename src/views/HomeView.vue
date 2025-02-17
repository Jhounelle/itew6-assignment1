<script setup>
import CardContainer from '@/components/CardContainer.vue';
</script>

<template>
  <div class="container">
    <CardContainer title="Learn More About Me" v-bind:card-height="400" v-bind:card-width="800" :is-title-centered="false">
      <h2>Hello, I am Jhounelle R. Casitas</h2>
      <div class="child-container">
        <CardContainer title="About Me" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Skills" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Contact" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
      </div>
    </CardContainer>
  </div>
</template>

<style scoped>
  body {
    margin: 0;
    padding: 0;
  }

  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    flex-wrap: wrap;
    padding: 20px;
  }

  .container h2 {
    text-align: center;
  }

  .child-container {
    display: flex;
    justify-content: center;
    gap: 10px;
    margin-top: 20px;
    flex-wrap: wrap;
  }
</style>
