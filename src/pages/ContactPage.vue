<template>
  <div class="page">

    <!-- NAVBAR -->
    <header class="navbar">

      <h2>SMK YADIKA SOREANG - Onlineshop</h2>

      <nav>
        <RouterLink to="/">Landing</RouterLink>
        <RouterLink to="/product">Product</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>

    </header>


    <!-- JUDUL -->
    <section class="title">

      <h1>Hubungi Kami</h1>

      <p>
        Silakan hubungi kami jika ada pertanyaan.
      </p>

    </section>


    <!-- CONTACT -->
    <section class="contact">

      <!-- INFO -->
      <div class="contact-info">

        <h2>Info Kontak</h2>

        <p>
          📍 <strong>Alamat</strong><br>
          Jl. Pendidikan No. 1, Soreang, Kab. Bandung
        </p>

        <p>
          📞 <strong>Telepon</strong><br>
          (022) 123-4567
        </p>

        <p>
          ✉️ <strong>Email</strong><br>
          yadika@smk.sch.id
        </p>

      </div>


      <!-- FORM -->
      <div class="form-box">

        <h2>Kirim Pesan</h2>

        <form>

          <label>Nama</label>

          <input
            type="text"
            placeholder="Nama kamu"
          >


          <label>Email</label>

          <input
            type="email"
            placeholder="email@contoh.com"
          >


          <label>Pesan</label>

          <textarea
            placeholder="Tulis pesan..."
          ></textarea>


          <button type="submit">
            Kirim
          </button>

        </form>

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


/* NAVBAR */

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
  text-decoration: none;

  color: #333;
}

nav a:hover {
  color: #405de6;
}


/* JUDUL */

.title {
  max-width: 1100px;

  margin: auto;

  padding: 40px;

  text-align: center;

  color: white;

  background: linear-gradient(
    120deg,
    #294a91,
    #405de6
  );

  border-radius: 8px;
}

.title h1 {
  margin-bottom: 10px;
}


/* CONTACT */

.contact {
  max-width: 950px;

  margin: 40px auto;

  padding: 0 20px;

  /* CLUE 2 KOLOM */

  display: flex;

  gap: 40px;

  align-items: flex-start;
}


/* INFO */

.contact-info {
  flex: 1;

  padding: 20px;
}

.contact-info h2 {
  color: #294a91;
}

.contact-info p {
  margin: 25px 0;

  color: #666;

  line-height: 1.5;
}


/* FORM */

.form-box {
  flex: 1;

  padding: 25px;

  background: white;

  /* CLUE */

  border-radius: 15px;

  /* CLUE */

  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
}

.form-box h2 {
  margin-top: 0;

  color: #294a91;
}

form {
  display: flex;

  flex-direction: column;

  gap: 8px;
}

label {
  font-size: 14px;

  font-weight: bold;
}

input,
textarea {
  padding: 12px;

  /* CLUE */

  border-radius: 8px;

  border: 1px solid #ddd;

  font-family: Arial, sans-serif;
}

textarea {
  min-height: 100px;

  resize: vertical;
}

input:focus,
textarea:focus {
  outline: none;

  border-color: #405de6;
}


/* TOMBOL */

button {
  margin-top: 10px;

  padding: 12px;

  border: none;

  /* CLUE */

  border-radius: 999px;

  background: #405de6;

  color: white;

  font-weight: bold;

  cursor: pointer;
}

button:hover {
  background: #294a91;
}


/* FOOTER */

footer {
  margin-top: 40px;

  padding: 25px;

  background: white;

  border-top: 1px solid #ddd;

  color: #666;
}


/* HP */

@media (max-width: 700px) {

  .navbar {
    height: auto;

    padding: 20px;

    flex-direction: column;

    gap: 15px;
  }

  .contact {
    flex-direction: column;
  }

  .contact-info,
  .form-box {
    width: 100%;
  }

}

</style>