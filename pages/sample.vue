<template>
  <div>
    <AtomsPrimaryButton
      :handle-click="handleClick"
      title="Add 1"
      @addNumber="handleClick"
    />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'SamplePage',
  data: () => ({
    count: 0,
  }),
  methods: {
    handleClick() {
      alert('Hello World')
    },
  },
})
</script>
