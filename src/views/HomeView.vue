<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <button>test</button>
    <button @click="goToDayBook" class="btn btn-primary">test</button>
    </div>
</template>

<script>

export default {
  name: 'HomeView',
  components: {
  },
  methods:{
    goToDayBook(){
      this.$router.push({name:'no-entry'})
    }
  }
}
</script>
