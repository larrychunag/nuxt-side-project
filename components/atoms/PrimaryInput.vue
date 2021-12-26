<template>
  <div>
    <b-form-group :label="label" :description="description">
      <b-form-input
        v-model="innerInputValue"
        :type="type"
        :placeholder="placeholder"
        :required="required ? true : false"
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
    },
    description: {
      type: String,
    },
    type: {
      type: String,
    },
    inputValue: {
      type: String,
    },
    placeholder: {
      type: String,
    },
    required: {
      type: Boolean,
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
