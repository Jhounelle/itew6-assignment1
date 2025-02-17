<script setup>
import CardContainer from '@/components/CardContainer.vue';
</script>

<template>
  <div class="container">
    <CardContainer title="Jhounelle R. Casitas" v-bind:card-height="400" v-bind:card-width="800" :is-title-centered="true">
      <div class="child-container">
        <CardContainer title="21 Years Old" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Developer" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Audiophile" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Technician" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="PC Gamer" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
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

  .child-container {
    display: flex;
    justify-content: center;
    gap: 10px;
    margin-top: 20px;
    flex-wrap: wrap;
  }
</style>
