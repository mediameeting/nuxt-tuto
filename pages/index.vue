<template>
  <v-layout
    justify-space-between
    row
    wrap
  >
    <v-flex
      v-for="(card, index) in cards"
      :key="index"
      xs4
    >
      <card
        :title="card.title"
        :text="card.text"
        :img="card.img"
      />
    </v-flex>
  </v-layout>
</template>

<script>
import Card from '@/components/Card'
export default {
  components: { Card },
  data: () => ({
    cards: [
      {
        title: 'Titre 1',
        text: 'text',
        img: 'https://cdn.pixabay.com/photo/2016/12/13/05/15/puppy-1903313__480.jpg'
      },
      {
        title: 'Titre 2',
        text: 'text',
        img: 'https://cdn.pixabay.com/photo/2018/05/07/10/48/husky-3380548__480.jpg'
      },
      {
        title: 'Titre 3',
        text: 'text',
        img: 'https://cdn.pixabay.com/photo/2016/01/19/17/41/friends-1149841__480.jpg'
      }
    ]
  })
}

</script>
