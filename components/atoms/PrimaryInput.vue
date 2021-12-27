<template>
  <div>
    <b-form-group :label="label" :description="description">
      <b-form-input
        v-model="innerInputValue"
        :type="type"
        :placeholder="placeholder"
      ></b-form-input>
    </b-form-group>
  </div>
</template>

<script>
export default {
  name: 'PrimaryCard',
  model: {
    prop: 'model',
    event: 'change',
  },
  props: {
    label: {
      type: String,
      default: '',
    },
    description: {
      type: String,
      default: '',
    },
    type: {
      type: String,
      default: 'text',
    },
    inputValue: {
      type: String,
      default: '',
    },
    placeholder: {
      type: String,
      default: 'Please enter',
    },
  },
  computed: {
    innerInputValue: {
      get() {
        return this.$props.inputValue
      },
      set(value) {
        this.$emit('change', value)
      },
    },
  },
}
</script>

<style lang="scss"></style>
