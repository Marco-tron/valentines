
<template>
  <div class="container bg-red-200">
    <div v-if="index === 0" @click="index++" class="flex flex-col items-center cursor-pointer">
      <h1 class="title">
        Feliz dia dos namorados!
      </h1>
      <div>
          <img class="heart" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/Heart_coraz%C3%B3n.svg/1200px-Heart_coraz%C3%B3n.svg.png" alt="">
      </div>
      <div>
          ps: dá uma clicada pra ver mais
      </div>
    </div>
    <div v-if="index === 1" @click="index++" class="flex flex-col items-center cursor-pointer">
      <h1 class="title">
        Fernanda, ja fazem 2 anos desde que nos conhecemos
      </h1>
      <div>
          <img class="heart" src="~/static/us.jpeg" alt="">
      </div>
    </div>
    <div v-if="index === 2" @click="index++" class="flex flex-col items-center cursor-pointer">
      <h1 class="title">
        E sei que quero passar toda a vida com você
      </h1>
      <div>
          <img class="heart" src="~/static/old-us.PNG" alt="">
      </div>
    </div>
    <div v-if="index === 3" @click="index++" class="flex flex-col items-center cursor-pointer">
      <h1 class="title">
        Sei que é pouco mas é minha mensagem pra você
      </h1>
      <div>
          <img class="heart" src="~/static/you.PNG" alt="">
      </div>
    </div>
    <div v-if="index === 4" @click="index++" class="flex flex-col items-center cursor-pointer">
      <h1 class="title">
        TE AMO!
      </h1>
      <div>
          <img class="heart" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/Heart_coraz%C3%B3n.svg/1200px-Heart_coraz%C3%B3n.svg.png" alt="">
      </div>
    </div>
    <div v-if="index === 5"  class="flex flex-col items-center cursor-pointer">
      <h1 class="title">
        É ISSO :)
      </h1>
    </div>
  </div>
</template>

<script>

export default {
  components: {
  },
  data () {
      return {
          index: 0
      }
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 64px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.heart {
    height: 600px;
}
.links {
  padding-top: 15px;
}
</style>
