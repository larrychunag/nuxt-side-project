<template>
  <div>
    <b-form>
      <AtomsPrimaryInput v-model="form.title" label="title" />
      <AtomsPrimaryInput v-model="form.description" label="description" />
      <AtomsPrimaryCard :title="form.title" :description="form.description" />
      <div class="flex-container">
        <AtomsPrimaryButton class="mr-1" title="create" />
        <AtomsPrimaryButton class="mr-1" title="delete" variant="danger" />
      </div>
    </b-form>
  </div>
</template>

<script>
export default {
  name: 'TheForm',
  props: {},
  data: () => {
    return {
      form: {
        title: '',
        description: '',
      },
    }
  },
  methods: {},
}
</script>

<style lang="scss">
.flex-container {
  display: flex;
  flex-direction: row;
}
</style>
