<template>
  <div class="home">
    <img alt="MDB logo" src="../assets/logo-mdb-vue-small.png">
    <Join />
  </div>
</template>

<script>
// @ is an alias to /src
import Join from '@/components/Join.vue'

export default {
  name: 'home',
  components: {
    Join
  }
}
</script>
