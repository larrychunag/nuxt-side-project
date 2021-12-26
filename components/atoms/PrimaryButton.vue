<template>
  <div>
    <b-button :variant="variant" @click="handleClick()">{{ title }}</b-button>
  </div>
</template>

<script>
export default {
  name: 'PrimaryButton',
  props: {
    handleClick: Function,
    title: String,
    variant: String,
  },
  methods: {},
}
</script>

<style lang="scss"></style>
