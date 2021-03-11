<template>
  <button @click="handleClick">{{ texto }}</button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    texto: String,
  },
  methods: {
    handleClick() {
      this.$emit('onClick');
    }
  }
}
</script>
