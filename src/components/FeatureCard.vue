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

