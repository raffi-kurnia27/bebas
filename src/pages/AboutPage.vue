<template>
  <div class="page">

    <section class="title">
      <h1>Tentang Kami</h1>
      <p>Mengenal lebih dekat Yadika Onlineshop.</p>
    </section>

    <section class="story">

      <div>
        <h2>Cerita Kami</h2>

        <p>
          Onlineshop ini dikelola langsung oleh siswa
          SMK Yadika Soreang jurusan PPLG.
        </p>

        <p>
          Kami membuat toko online ini untuk membantu
          siswa mendapatkan perlengkapan sekolah dengan
          mudah dan harga terjangkau.
        </p>
      </div>


      <div class="story-image">
        🛍️
      </div>

    </section>

    <section class="team">

      <h2>Tim Kami</h2>

      <div class="team-list">

        <div class="team-card">
          <div class="avatar">A</div>
          <h3>Ahmad</h3>
          <p>Ketua Tim</p>
        </div>

        <div class="team-card">
          <div class="avatar">S</div>
          <h3>Siti</h3>
          <p>Desain UI</p>
        </div>

        <div class="team-card">
          <div class="avatar">R</div>
          <h3>Rian</h3>
          <p>Programmer</p>
        </div>

      </div>

    </section>


    <footer>
      © 2026 SMK Yadika Soreang — Onlineshop Sekolah
    </footer>

  </div>
</template>


<style scoped>

* {
  box-sizing: border-box;
}

.page {
  min-height: 100vh;
  background: #f5f8ff;
  font-family: Arial, sans-serif;
  color: #263858;
}

.navbar {
  max-width: 1100px;
  height: 75px;

  margin: auto;
  padding: 0 25px;

  display: flex;
  align-items: center;
  justify-content: space-between;

  background: white;
}

.navbar h2 {
  color: #294a91;
  font-size: 20px;
}

nav {
  display: flex;
  gap: 25px;
}

nav a {
  color: #333;
  text-decoration: none;
}

nav a:hover {
  color: #405de6;
}

.title {
  max-width: 1100px;

  margin: auto;

  padding: 45px;

  text-align: center;

  color: white;

  background: linear-gradient(
    120deg,
    #294a91,
    #405de6
  );

  border-radius: 8px;
}

.story {
  max-width: 950px;

  margin: 40px auto;

  padding: 0 20px;

  display: flex;

  align-items: center;

  gap: 40px;
}

.story > div {
  flex: 1;
}

.story p {
  color: #666;
  line-height: 1.6;
}

.story-image {
  height: 220px;

  display: flex;

  align-items: center;
  justify-content: center;

  background: #e7ebff;

  border-radius: 15px;

  font-size: 70px;
}

.team {
  max-width: 1000px;

  margin: auto;

  padding: 35px 20px;

  text-align: center;

  background: #eef3fb;
}

.team-list {
  display: flex;

  gap: 20px;

  flex-wrap: wrap;

  justify-content: center;
}

.team-card {
  width: 200px;

  padding: 25px;

  background: white;

  border-radius: 12px;

  box-shadow: 0 4px 12px rgba(0,0,0,0.1);

  transition: 0.3s;
}

.team-card:hover {
  transform: translateY(-7px);
}

.avatar {
  width: 60px;
  height: 60px;

  margin: auto;

  display: flex;

  align-items: center;
  justify-content: center;

  border-radius: 50%;

  background: #405de6;

  color: white;

  font-size: 25px;
  font-weight: bold;
}

footer {
  margin-top: 40px;

  padding: 25px;

  background: white;

  border-top: 1px solid #ddd;

  color: #666;
}

</style>