<template>
  <Header @changeTitle="ubahText" :text="text" />
</template>

<script>
import Header from "@/components/Header.vue";

export default {
  name: 'App',
  data() {
    return {
      text: "Ini adalah text dari app.vue"
    }
  },
  components: {
    Header
  },
  methods: {
    ubahText(newText){
      this.text = newText
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
