<template>
  <div class="container-fluid">
    <div class="row mt-4 d-flex justify-content-evenly">
      <div class="col-lg-4">
        <div class="card">
          <div class="card-body">
            <img src="~/assets/img/cover4.jpg" width="220px" height="340px" class="cover" alt="cover4">
          </div>
        </div>
      </div>
      <div class="col-4">
        <p>Penulis : Nurmala</p>
        <p>Penerbit : PT Gramedia Widiasarana</p>
        <p>Tahun terbit : 2023</p>
      </div>
    </div>
    <div class="row mt-5">
      <h2>Sinopsis</h2>
      <p class="mt-3"> Rijal adalah seorang mahasiswa baru yang berasal dari Pulau Sumatra. Ia merantau ke UI untuk kuliah. Sebagai anak lelaki tunggal, meninggalkan orangtua sangatlah berat. Hari-harinya dipenuhi dengan rindu pada orangtua dan masa kecilnya. Namun demi mengejar impiannya, ia harus melewati masa-masa itu.
Selama di Depok, Rijal yang sejak kecil didik oleh orangtuanya tentang kebijaksanaan hidup dan pengetahuan agama, dihadapkan pada perasaan yang tak terbendung. Ia tertarik pada Laras pada pandangan pertama saat Rijal menginjakkan kaki di UI.
Pada hari-hari setelahnya, Rijal harus memutuskan pada pilihan yang sama-sama sulit. Di satu sisi Rijal tidak ingin membuat orangtuanya kecewa, di sisi lain ia tidak ingin melepaskan kesempatan atas nama cinta.</p>
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