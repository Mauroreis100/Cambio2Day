<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      You’ve successfully created a project with
      <a href="https://vitejs.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>.
    </h3>
    <div class="calculator">
      <div class="card">
        <div class="moeda">
          <p>Quantia</p>
          <input></input>
        </div>
        <br>
        <slot>><</slot>
        <div class="moeda">
          <p>Quantia</p>
          <input></input>
        </div>
        </div>
        <button>Converter</button>
        </div>
  </div>
</template>

<style scoped>


.calculator{
  padding: 100px;
  display: flex;
  justify-content: center;
  background-color: rgb(245, 1, 1);

}
.moeda{
  display: flex;
  flex-direction: column;
  
}
.card{
  display: flex;
justify-content: space-between;

}
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
  
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: center;
  }
}
</style>
