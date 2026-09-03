
<template>
    <main>
        <section class="hero">
            <h1>selamat Datang di lah onlineshop</h1>
            <p>Belanja Gampang dapat uang susah</p>
        </section>

        <video controls width="480" muted loop>
            <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4" />
            browser kamu tidak mendukung pemutaran video ini
        </video>
        <RouterLink to="/Product"><button>lihat produk</button></RouterLink>
    </main>
</template>
<script>

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