<template>
  <div class="container-fluid">
    <div class="row my-5">
      <div class="col-lg-6">
      <nuxt-link to="/pengunjung/tambah">
          <div class="card bg-pengunjung rounded-5">
            <div class="card-body">
              <h2>pengunjung</h2>
              </div>
            </div>
          </nuxt-link>
        </div>
        <div class="col-lg-6">
          <nuxt-link to="/buku">
            <div class="card bg-buku rounded-5">
              <div class="card-body">
                <h2>Cari Buku</h2>
              </div>
            </div>
          </nuxt-link>
        </div>
      </div>

      <div class="row my-5">
      <div class="col-lg-6">
          <div class="card pengunjung rounded-5">
            <div class="card-body">
              <h1>{{ jumlahp }}</h1>
            <h2>Pengunjung</h2>
              </div>
            </div>
    
        </div>
        <div class="col-lg-6">

            <div class="card buku rounded-5">
              <div class="card-body">
                <h1 >{{ jumlahb }}</h1>
                <h2 >Buku</h2>
              </div>
            </div>

        </div>
      </div>
    </div>
</template>

<script setup>
useHead({
  title: "PERPUS DIGITAL",
  meta: [
    {
      name: "description",
      content: "Selamat datang diperpus digital SMKN 4",
    },
  ],
});
const supabase = useSupabaseClient();

const jumlahp = ref(0);

const jumlahb = ref(0);

const pengunjung = async () => {
  const { data, error, count } = await supabase.from("pengunjung").select("*", { count: "exact" });
  if (count) jumlahp.value = count;
};

const buku = async () => {
  const { data, error, count } = await supabase.from("buku").select("*", { count: "exact" });
  if (count) jumlahb.value = count;
};

onMounted(() => {
  pengunjung();
  buku();
});
</script>

<style scoped>
.card {
  height:250px;
  box-shadow: 1px 1px 10px #424242;
}
.card.bg-pengunjung {
  background-image: url('../assets/img/bg-home-kunjungan.jpeg');
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
}
.card.bg-buku {
  background: url('../assets/img/bg-home-cari-buku.jpg');
  background-size: cover;
}
.card.buku {
  background-color: #1442d8;
  color: white;
}
.card.pengunjung {
  background-color: #1442d8;
  color: white;
}

</style>