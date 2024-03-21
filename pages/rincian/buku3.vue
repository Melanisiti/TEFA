<template>
  <div class="container-fluid">
    <div class="row mt-4 d-flex justify-content-evenly">
      <div class="col-lg-4">
        <div class="card">
          <div class="card-body">
            <img src="~/assets/img/cover3.jpg" width="220px" height="340px" class="cover" alt="cover3">
          </div>
        </div>
      </div>
      <div class="col-4">
        <p>Penulis : Asma Nadia</p>
        <p>Penerbit : PT Pustaka Abdi Bangsa</p>
        <p>Tahun terbit : 2022</p>
      </div>
    </div>
    <div class="row mt-5">
      <h2>Sinopsis</h2>
      <p class="mt-3"> Beberapa tahun setelah pernikahan Meirose (Marsha Timothy) dan Pras (Fedi Nuril), Meirose terus berjuang untuk menciptakan kembali surga dunia dalam rumah tangga yang dibangunnya bersama Pras. Demi kedua anaknya, Akbar dan Nadia, Meirose juga berusaha menjadi seorang Ibu yang memberikan kebahagiaan untuk keluarganya. Namun, ujian kembali hadir setelah munculnya Ray (Reza Rahadian), pria yang dulu menghamili dan meninggalkannya. Meirose dihadapkan dengan berbagai pilihan sulit karena Ray berusaha untuk kembali masuk ke kehidupannya. Sebagai seorang ayah, Ray berusaha untuk dekat dengan putranya. Meirose tentunya tak ingin menjauhkan Akbar dari ayah kandungnya sendiri. Di sisi lain, keberadaan Ray membuat Pras kurang nyaman. Setelah kedatangan Ray, Pras dan Meirose jadi sering terlibat adu mulut. Pras bahkan tega mendiamkan istrinya sendiri selama berhari-hari. Akankah Meirose berhasil menghadapi rintangan dan menciptakan surga dunia di dalam rumah tangganya dengan Pras?</p>
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