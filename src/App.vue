<template>
<div>
  <div class="app">
    <b-table striped hover :items="items"></b-table>
    <b-pagination
      v-model="currentPage"
      :total-rows="rows"
      :per-page="perPage"
      aria-controls="my-table"
    ></b-pagination>
  </div>
</div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data() {
      return {
        items: [
          { 일련번호: 40, 제목: 'Dickerson', 등록일: 'Macdonald' },
          { 일련번호: 21, 제목: 'Larsen', 등록일: 'Shaw' },
          { 일련번호: 89, 제목: 'Geneva', 등록일: 'Wilson' },
          { 일련번호: 38, 제목: 'Jami', 등록일: 'Carney' }
        ]
      }
    }
}
</script>

<style>
.app {
  min-width:500px;
  margin: 60px auto;
  border: 1px solid red;
}
</style>
