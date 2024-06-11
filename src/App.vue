<script setup>
import MainCard from './components/MainCard.vue'
import NavBar from './components/NavBar.vue'
</script>

<template>
  <header>
    <NavBar/>
  </header>

  <main>
   
    <MainCard msg="Convesor de Moedas" />
  </main>
</template>

<style scoped>
header {
  display: flex;
position: sticky;
position: -webkit-sticky;
  line-height: 1.5;
  background:rgb(70, 146, 70);
}
main{
  padding-top: 125px;
  background-color: greenyellow;
  padding-inline: 24px;
}

</style>
