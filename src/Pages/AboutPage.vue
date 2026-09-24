<template>
    <main>
        <h1>About Us</h1>
        <p>Welcome to our online shop! We are dedicated to providing you with the best shopping experience.</p>
        <section class="team">
            <TeamCard
                v-for="member in teamMembers"
                :key="member.id"
                :name="member.name"
                :role="member.role"
                :image="member.image"
            />
        </section>
    </main>
</template>
<script setup>
import TeamCard from '../components/TeamCard.vue';
const teamMembers = [
    { name: 'johan', role: 'Developer', image: 'https://avatars.githubusercontent.com/u/12345678?v=4' },
    { name: 'Jane tricker', role: 'Back-end Developer', image: 'https://avatars.githubusercontent.com/u/87654321?v=4' },
    { name: 'John Smith', role: 'UI/UX Designer', image: 'https://avatars.githubusercontent.com/u/56789012?v=4' }
]
</script>