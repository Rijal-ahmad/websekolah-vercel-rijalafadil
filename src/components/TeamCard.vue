<template>
    <div class="TeamCard">
        <img :src="image" :alt="name">
        <h3 class="name">{{ name }}</h3>
        <p class="role">{{ role }}</p>

    </div>
</template>
<script setup>
defineProps({
    id: {
        type: Number,
        default: 0
    },
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
<style scoped>
.TeamCard {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: rgb(27, 238, 220);
    padding: 20px;
    gap: 10px;
    text-align: center;
    box-shadow: 0px 4px 15px rgba(0, 0, 0,0.15);
    border-radius: 10px;
}
</style>
