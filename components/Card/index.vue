<template>
  <v-card>
    <v-img
      :src="img"
      aspect-ratio="1.5"
    />
    <v-card-title> {{ title }} </v-card-title>
    <v-card-text> {{ text }} </v-card-text>
    <v-card-actions>
      <v-btn> play </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'no title',
      required: true
    },
    text: {
      type: String,
      default: 'no text',
      required: true
    },
    img: {
      type: String,
      default: '',
      required: true
    }
  }
}
</script>

<style lang="scss">

</style>
