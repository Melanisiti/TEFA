<template>
  <div class="container-fluid">
    <div class="row mt-4 d-flex justify-content-evenly">
      <div class="col-lg-4">
        <div class="card">
          <div class="card-body">
            <img src="~/assets/img/cover2.jpg" width="220px" height="340px" class="cover" alt="cover2">
          </div>
        </div>
      </div>
      <div class="col-4">
        <p>Penulis : Agnes Davonar</p>
        <p>Penerbit : Falkon Pubilshing</p>
        <p>Tahun terbit : 2008</p>
      </div>
    </div>
    <div class="row mt-5">
      <h2>Sinopsis</h2>
      <p class="mt-3"> kisah pilu tentang kehidupan kakak beradik yatim piatu, Anton dan Angel. Dimana keduanya terjebak dalam suatu sindikat yang memanfaatkan anak-anak terlantar untuk menjadi pengemis jalanan. Di usia mereka yang masih sangat kecil, mereka diperbudak untuk menjadi mesin uang tanpa kenal waktu. Keduanya tidak pernah mengenal indahnya masa kecil. Hingga satu peristiwa Angel mengalami kecelakaan di jalan raya. Ketika Angel sadar, ia sudah ditinggalkan seorang diri di rumah sakit. Dan sejak saat itulah Angel terpisahkan dengan Anton. Ia tidak pernah tahu lagi dimana keberadaan Abangnya. 15 tahun berlalu, di Sydney, Australia. Berkat keluarga angkatnya yang baik hati, Angel tumbuh menjadi perempuan cantik dan pandai. Ia berhasil mewujudkan mimpinya menjadi seorang Pengacara. Disana Angel bertemu dengan Martin seorang dokter muda asal Indonesia yang baik hati dan membuatnya jatuh cinta. Hidupnya kini diliputi kebahagiaan. Tapi meski demikian Angel tetap dihantui oleh masa lalunya. Ia tidak pernah bisa berhenti memikirkan Anton. Ditengah hidupnya yang penuh kebahagiaan dan rencananya untuk menikah dengan Martin, Angel mengambil keputusan untuk kembali ke Jakarta untuk menyelesaikan dulu masa lalunya, mencari keberadaan sang Abang.</p>
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