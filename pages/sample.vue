<template>
  <div>
    <AtomsPrimaryInput
      v-model="value"
      title="sample"
      label="please enter"
      description="sample card"
      required="true"
    />
  </div>
</template>
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'SamplePage',
  data: () => {
    return {
      value: '',
    }
  },
  methods: {},
})
</script>
