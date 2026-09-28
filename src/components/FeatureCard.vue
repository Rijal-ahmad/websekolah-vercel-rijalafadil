<template>
    <div class="FeatureCard flex flex-col items-center overflow-hidden bg-[#8282FF]; padding: 30px; gap: 10px; text-align: left; box-shadow: 0px 4px 15px rgba(0, 0, 0,0.15); border-radius: 10px;">
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
