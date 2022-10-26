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
    <div :style="{ 'background-color': 'black', 'padding': '1rem', 'display': 'flex', 'border-radius': '0.25rem', 'justify-content': 'center', 'align-items': 'center', 'margin-top': '1rem' }" >
      <span :style="{ 'font-weight': 'bolder', 'color': 'white' }" >Powered by: </span>
      <img alt="Vue logo" class="logo" src="../assets/pantheon.png" :style="{ 'display': 'inline-block;', 'height': '200', 'width': '100' }" />
  </div>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
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
    text-align: left;
  }
}
</style>
