<template>
  <div class="container">

    <section class="hero">
      <h1>
        Belanja Perlengkapan Sekolah,<br>
        Gampang & Terpercaya
      </h1>

      <p>
        Dari kaos, topi sampai tas sekolah — semua ada di satu tempat.
      </p>

      <button class="btn">
        Lihat Produk
      </button>
    </section>

    <!-- FITUR -->
    <section class="features">

      <div class="card">
        <div class="icon">😆</div>
        <h3>Kualitas Terjamin</h3>
        <p>
          Bahan pilihan dengan kualitas yang nyaman.
        </p>
      </div>

      <div class="card">
        <div class="icon">💵</div>
        <h3>Harga Bersahabat</h3>
        <p>
          Harga ramah di kantong siswa.
        </p>
      </div>

      <div class="card">
        <div class="icon">🏫</div>
        <h3>Ambil di Sekolah</h3>
        <p>
          Tidak perlu antre, ambil di koperasi.
        </p>
      </div>

    </section>

  </div>
 
  <main> 
    <h1>Selamat Datang di Onlineshop Sekolah</h1> 
    <p>Belanja gampang, sekolah senang.</p> 
  
    <video controls width="480" muted loop> 
      <source src="/video/promo-toko.mp4" type="video/mp4" /> 
      Browser kamu tidak mendukung pemutaran video. 
    </video> 
  </main> 
</template> 
  
<style scoped> 
video { 
  margin-top: 16px; 
  border-radius: 10px; 
  display: block; 
} 
</style>


<script>
export default {
  name: "App"
}
</script>


<style>
/* =========================
   DASAR
========================= */

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #eef5f4;
}

/* HERO */
.hero {
  background: linear-gradient(
    135deg,
    #00a896,
    #05668d
  );

  padding: 100px 30px;
  text-align: center;

  color: white;
  min-height: 400px;
  border-radius: 10px;
}

.hero h1 {
  margin-bottom: 20px;
}

.hero p {
  margin-bottom: 30px;
}

/* TOMBOL */
.btn {
  border: none;

  background: #ffd166;
  color: #333;

  padding: 12px 30px;

  border-radius: 999px;

  font-weight: bold;
  cursor: pointer;

  box-shadow: 0 5px 12px rgba(0, 0, 0, 0.2);
}

.btn:hover {
  transform: scale(1.05);
}

/* FITUR */
.features {
  display: flex;
  justify-content: center;

  gap: 15px;
  flex-wrap: wrap;

  padding: 50px 20px;
}

/* CARD */
.card {
  width: 210px;
  min-height: 130px;

  background: white;

  text-align: center;

  padding: 25px 15px;

  border-radius: 12px;

  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.1);
}

.icon {
  font-size: 28px;
  margin-bottom: 10px;
}

.card h3 {
  font-size: 15px;
  margin: 5px 0 8px;
}

.card p {
  font-size: 11px;
  color: #777;
  line-height: 1.5;
}

</style>