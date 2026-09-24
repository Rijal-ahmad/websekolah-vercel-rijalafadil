<template>
        <section class="hero">
            <h1>selamat Datang di lah onlineshop</h1>
            <p>Belanja Gampang dapat uang susah</p>
            
            <video controls width="480" muted loop>
                <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4" />
                browser kamu tidak mendukung pemutaran video ini
            </video>
            <RouterLink to="/Product"><button>lihat produk</button></RouterLink>
        </section>
        <section class="Features">
            <FeatureCard
                v-for="feature in features"
                :key="feature.title"
                :icon="feature.icon"
                :title="feature.title"
                :description="feature.description"
            />
        </section>
</template>
<script setup>
import FeatureCard from '../components/FeatureCard.vue';

const features = [
    {
        icon: '🛒',
        title: 'Belanja mudah',
        description: 'Temukan berbagai produk dengan cepat dan mudah.'
    },
    {
        icon: '🚚',
        title: 'Pengiriman cepat',
        description: 'Pesanan dikirim dengan aman sampai ke tujuan.'
    },
    {
        icon: '💳',
        title: 'Pembayaran aman',
        description: 'Nikmati proses pembayaran yang praktis dan terpercaya.'
    }
];

</script>

<style scoped>
 .card {
    display: flex;
    flex-direction: column;
    background-color: antiquewhite;
    padding: 30px;
    gap: 10px;
    text-align: left;
    box-shadow: 0px 4px 15px rgba(0, 0, 0,0.15);
    border-radius: 10px;
    flex: box;
    
 }
    .hero {
        text-align: center;
        padding: 20px;
        background: linear-gradient(to right, rgb(92,92,240), rgb(130,130,255));
        flex: wrap;
        color: antiquewhite;
    }
    video {
        margin-bottom: 25px;
        border-radius: 10px;
        display: block;
    }
    button {
        display: block;
        margin: 15px auto;

    }
    
</style>