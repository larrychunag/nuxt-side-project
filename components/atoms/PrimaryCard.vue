<template>
  <div>
    <b-card
      :title="title"
      :img-src="imgSrc"
      :img-alt="imgAlt"
      img-top
      style="max-width: 20rem"
      class="mb-2"
    >
      <b-card-text>
        {{ description }}
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'PrimaryCard',
  props: {
    imgSrc: {
      type: String,
      default: '/no-image-icon.png',
    },
    imgAlt: {
      type: String,
      default: 'sample',
    },
    title: String,
    description: {
      type: String,
    },
  },
  methods: {},
}
</script>

<style lang="scss"></style>
