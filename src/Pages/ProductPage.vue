<script setup>
import ProductCard from '../components/ProductCard.vue';
const daftarProduk = [
    {id : 1, nama: 'pulpen', harga: 110000, gambar: 'https://th.bing.com/th/id/OIP.ceA-nGCs-J15JLTXKne7ZwHaHa?w=195&h=195&c=7&r=0&o=7&pid=1.7&rm=3'},
    {id : 2, nama: 'baju', harga: 210000,  gambar: 'https://th.bing.com/th/id/OIP.kD-INauJ9ZytHjKD3W7RKwHaHa?w=197&h=197&c=7&r=0&o=7&pid=1.7&rm=3' },
    {id : 3, nama: 'jaket', harga: 300000, gambar: 'https://th.bing.com/th/id/OIP.mpdtIDtf2BFu3BjHP6lPEAHaIM?w=194&h=214&c=7&r=0&o=7&pid=1.7&rm=3' },
]
</script>


<template>
    <main>
        <h1>Produk Kami</h1>
        <div class="grid">
            <ProductCard 
                v-for="produk in daftarProduk" 
                :key="produk.id"
                :nama="produk.nama"
                :harga="produk.harga"
                :gambar="produk.gambar"
            />
        </div>
    </main>
</template>

<style scoped>
.grid {
 display: flex;
 gap: 16px;
 flex-wrap: wrap;
 box-shadow: 0px, 0px,4px;
}

</style>
