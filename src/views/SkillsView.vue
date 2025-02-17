<script setup>
import CardContainer from '@/components/CardContainer.vue';
</script>

<template>
  <div class="container">
    <CardContainer title="My Skills" v-bind:card-height="600" v-bind:card-width="800" :is-title-centered="false">
      <div class="child-container">
        <CardContainer title="JavaScript" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="PHP" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Java" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="C#" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="C++" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Lua" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Python" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Node.js" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="Vue.js" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="React.js" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
        </CardContainer>
        <CardContainer title="TypeScript" v-bind:cardHeight="40" v-bind:cardWidth="150" :is-title-centered="true">
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
