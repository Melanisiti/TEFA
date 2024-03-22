<template>
  <div class="container-fluid">
    <div class="row mt-4 d-flex justify-content-evenly">
      <div class="col-lg-4">
        <div class="card">
          <div class="card-body">
            <img src="~/assets/img/cover1.jpg" width="220px" height="340px" class="cover" alt="cover1">
          </div>
        </div>
      </div>
      <div class="col-4">
        <p>Penulis : Tere Liye</p>
        <p>Penerbit : Mahaka Pubilshing</p>
        <p>Tahun terbit : 2012</p>
      </div>
    </div>
    <div class="row mt-5">
      <h2>Sinopsis</h2>
      <p class="mt-3"> Pada awalnya Putri yang selalu mengumbar-ngumbar kedekatannya dengan Rio. 
        Kedekatan itu hanya berlangsung di dunia maya. Dan sangat berbeda di dunia nyata. Mereka berdua jauh dari kata dekat.
Setelah Putri, Nana juga merasakan hal yang sama. 
Yang awalnya bahagia bisa dekat dengan Rio. 
Namun, lagi-lagi kedekatan itu hanya di dunia maya dan bahkan hanya sementara saja. 
Cerita tersebut sangat menguji pertemanan dua anak manusia yang dimabuk cinta tersebut.</p>
    </div>
    <nuxt-link to="/buku">
      <button type="button" class="btn btn-dark mt-5">Kembali</button>
    </nuxt-link>
  </div>
</template>

<style scoped>
.card {
  width: 255px;
  height: 370px;
  box-shadow: 1px 1px 10px #424242;
}
</style>

<script setup>
const supabase = useSupabaseClient()

const route = useRoute()
const buku = ref([])
</script>