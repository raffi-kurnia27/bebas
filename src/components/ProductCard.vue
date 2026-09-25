<script setup>
import { ref } from 'vue'
defineProps(['nama', 'harga', 'gambar'])
const gambarDipilih = ref(null)
function bukaPreview(src) {
  gambarDipilih.value = src
}
function tutupPreview() {
  gambarDipilih.value = null
}
function tambahKeKeranjang(nama) {
  const suara = new Audio('/audio/notifikasi.mp3')
  suara.play()
  alert(`${nama} ditambahkan ke keranjang!`)
}
</script>
 
<template>
  <div class="bg-white rounded-xl shadow-md p-4 hover:shadow-lg transition">
    <img :src="gambar" :alt="nama" @click="bukaPreview(gambar)"
         class="w-full h-40 object-cover rounded-lg cursor-pointer" />
    <h3 class="text-lg font-semibold mt-2">{{ nama }}</h3>
    <p class="text-gray-600">Rp {{ harga.toLocaleString('id-ID') }}</p>
    <button @click="tambahKeKeranjang(nama)"
            class="bg-blue-600 text-white px-4 py-2 rounded-lg mt-2 w-full hover:bg
blue-700">
      Tambah ke Keranjang
    </button>
  </div>
  <div v-if="gambarDipilih" class="fixed inset-0 bg-black/70 flex items-center justify
center cursor-zoom-out"
       @click="tutupPreview">
    <img :src="gambarDipilih" class="max-w-[80%] max-h-[80%] rounded-lg" />
  </div>
</template>