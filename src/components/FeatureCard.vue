<template>
    <div class="FeatureCard">
        <div class="Feature-icon">{{ icon }}</div>
        <h3 class="title">{{ title }}</h3>
        <p class="description">{{ description }}</p>
    </div>
</template>
<script setup>
defineProps ({
    icon: {
        type: String,
        default: '🖊'
    },
    title: {
        type: String,
        default: 'Feature'
    },
    description: {
        type: String,
        default: 'Description'
    }
})
</script>
<style scoped>
.FeatureCard {
    display: flex;
    flex-direction: column;
    background-color: rgb(4, 95, 12);
    padding: 30px;
    gap: 10px;
    text-align: left;
    box-shadow: 0px 4px 15px rgba(0, 0, 0,0.15);
    border-radius: 10px;
}
</style>
