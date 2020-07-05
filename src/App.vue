<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1 @click="clickCaption" :class="classCaption">{{ textCaption }}</h1>
  </div>
</template>

<script>

export default {
  name: 'App',
  data: () => {
    return {
      textCaption: 'Заголовок',
      classCaption: 'colorGreen'
    }
  },
  methods: {
    clickCaption: () => {
      console.log('Проверка связи')
    }
  },
  components: {

  }

}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1.colorGreen {
  color: green;
}
</style>
