<template>
  <div>
    <b-button :variant="variant" @click="handleClick()">{{ title }}</b-button>
  </div>
</template>

<script>
export default {
  name: 'PrimaryButton',
  props: {
    handleClick: {
      type: Function,
      required: true,
      default: () => {},
    },
    title: {
      type: String,
      required: true,
      default: '',
    },
    variant: {
      type: String,
      required: true,
      default: 'primary',
    },
  },
  methods: {},
}
</script>

<style lang="scss"></style>
