<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">BUKU</h2>
        <div class="my-3">
          <input v-model="keyword" type="search" class="form-control rounded-5" placeholder="Mau baca buku apa hari ini?">
        </div>

        <div class="my-3 text-muted">menampilkan 4 dari 4</div>
        <div class="row">
          <div v-for="(book,i) in books" :key="i" class="col-lg-2">
            <div class="card mb-3">
              <div class="card-body">
                <nuxt-link :to="`/buku/${book.id}`">
                <img :src="book.cover" class="cover" alt="cover 1">
              </nuxt-link>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <nuxt-link to="/">
    <button type="button" class="btn btn-primary btn-lg mt-4">KEMBALI</button></nuxt-link>
  </div>
</template>

<script setup>
const supabase = useSupabaseClient()

const books = ref([])

const getBooks = async () => {
  const {data, error } = await supabase.from('buku').select(`*, kategori(*)`)
  .ilike('judul', `%${keyword.value}%`)
  if(data) books.value = data
}

onMounted(() => {
  getBooks()
})

const keyword = ref ('')
</script>


<style scoped>
.card-body {
  width: 100%;
  height: 20em;
  padding: 0%;
}
.cover {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: 0 30%;
}
</style>