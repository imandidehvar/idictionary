<template>
  <div class="container">
    <div class="row">
      <div class="form-group col-12 mt-4">
        <label for="Term">Input Text</label>
        <input type="text" class="form-control" id="Term" placeholder="Enter text" @input="textChanged" v-model="text">
      </div>
    </div> 
  </div>
</template>

<script>
export default {
  name: 'text-input',
  data() {
    return {
      text: "",
    }
  },
  methods: {
    textChanged(event) {
      this.$emit("translate", event.data)
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
