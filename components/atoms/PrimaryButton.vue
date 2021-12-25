<template>
  <div>
    <b-button @click="handleClick()">{{ title }}</b-button>
  </div>
</template>

<script>
export default {
  name: 'PrimaryButton',
  props: {
    handleClick: Function,
    title: String,
  },
  methods: {},
}
</script>

<style lang="scss"></style>
