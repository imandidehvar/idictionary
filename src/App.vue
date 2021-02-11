<template>
<navbar></navbar>
<text-input @translate="translate"/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import TextInput from './components/TextInput.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    TextInput,
  },
  methods: {
    translate(text) {
      alert(text)
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

@import'~bootstrap/dist/css/bootstrap.css'
</style>
