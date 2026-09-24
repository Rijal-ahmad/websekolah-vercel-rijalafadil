<template>
    <div class="TeamCard">
        <img :src="image" :alt="name">
        <h3 class="name">{{ name }}</h3>
        <p class="role">{{ role }}</p>

    </div>
</template>
<script setup>
defineProps({
    name: {
        type: String,
        default: 'Nama Anggota'
    },
    role: {
        type: String,
        default: 'Peran Anggota'
    },
    image: {
        type: String,
        default: ''
    }
})
</script>
