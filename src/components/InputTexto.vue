<template>
  <div class="inputTexto">
    <input v-model="texto" type="text" v-on:input="handleInput()">
  </div>
</template>

<script>
export default {
  name: 'InputTexto',
  data: function() {
    return {
      texto: '',
    }
  },
  methods: {
    handleInput() {
      this.$emit('onChange', this.texto);
    }
  }
}
</script>
