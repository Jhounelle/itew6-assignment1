<script setup>
    const props = defineProps({
        title: String,
        subtitle: String,
        cardHeight: Number,
        cardWidth: Number,
        isTitleCentered: {
            type: Boolean,
            default: true,
        },
    });
</script>

<template>
  <div class="card" v-bind:style="{ height: `${cardHeight}px`, width: `${cardWidth}px` }">
    <div class="card-header" v-if="title">
      <h2 class="card-title" :class="{ 'title-center': isTitleCentered }">{{ title }}</h2>
      <p v-if="subtitle" class="card-subtitle">{{ subtitle }}</p>
    </div>
    <div class="card-body">
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>
    .card {
        background: #f8f9fa;
        border-radius: 12px;
        padding: 40px;
        transition: all 0.3s ease;
        border: 1px solid #e0e0e0;
    }

    .card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
    }

    .card-header {
        margin-bottom: 12px;
    }

    .card-title {
        font-size: 1.5rem;
        font-weight: bold;
        margin: 0;
    }

    .card-subtitle {
        font-size: 1rem;
        color: #666;
    }

    .title-center {
        text-align: center;
    }
</style>