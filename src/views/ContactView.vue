<script setup>
import CardContainer from '@/components/CardContainer.vue';
</script>

<template>
  <div class="container">
    <CardContainer title="My Contacts" v-bind:card-height="400" v-bind:card-width="800" :is-title-centered="false">
      <div class="child-container">
        <CardContainer title="" v-bind:cardHeight="50" v-bind:cardWidth="140" :is-title-centered="true">
            <a href="https://facebook.com/Jhounelle09" target="_blank">Facebook</a>
        </CardContainer>
        <CardContainer title="" v-bind:cardHeight="50" v-bind:cardWidth="140" :is-title-centered="true">
            <a href="https://instagram.com/tkt.nelle" target="_blank">Instagram</a>
        </CardContainer>
        <CardContainer title="" v-bind:cardHeight="50" v-bind:cardWidth="140" :is-title-centered="true">
            <a href="https://github.com/Jhounelle" target="_blank">Github</a>
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
        text-align: center;
    }

    a {
        text-decoration: none;
        color: #000000;
        font-weight: 600;
        font-size: 26px;
        padding: 10px 15px;
        border-radius: 8px;
        transition: all 0.3s ease-in-out;
        display: inline-block;
    }

    a:hover {
        /* background-color: #007bff; 
        color: white; */
        box-shadow: 0 4px 8px rgba(112, 112, 112, 0.3);
        transform: translateY(-2px);
    }

    a::after {
        content: "";
        display: block;
        width: 0;
        height: 3px;
        background: #b4b4b4;
        transition: width 0.3s ease-in-out;
        margin-top: 4px;
    }

    a:hover::after {
        width: 100%;
    }
</style>
