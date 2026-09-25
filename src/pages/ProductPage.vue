<script setup>
import ProductCard from '../components/ProductCard.vue'
 
const daftarProduk = [
  { id: 1, nama: 'Kaos Sekolah', harga: 75000, gambar: 
'https://i.pinimg.com/1200x/ed/e2/02/ede202cf23920e33a83c117bcf11f24b.jpg' },
  { id: 2, nama: 'Topi Sekolah', harga: 35000, gambar: 
'https://i.pinimg.com/736x/5c/b4/52/5cb4521387f8402ac1db29bc8a6ea301.jpg' },
  { id: 3, nama: 'Tas Sekolah', harga: 120000, gambar: 
'https://i.pinimg.com/736x/d5/7b/46/d57b46eb80ffdc194d5d3156ca338f49.jpg' },
]
</script>
 
<template>
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 p-6">
    <ProductCard
      v-for="produk in daftarProduk"
      :key="produk.id"
      :nama="produk.nama"
      :harga="produk.harga"
      :gambar="produk.gambar"
    />
  </div>
</template>
 
<style scoped>
.grid {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}
</style>