<script setup>
import Card from './Card.vue'
defineProps({
  items: Array
})
const onclickAdd = () => {
  alert('Add!')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      v-for="item in items"
      :key="item.id"
      :title="item.title"
      :price="item.price"
      :imageUrl="item.imageUrl"
      :onclickAdd="onclickAdd"
      :isFavorite="item.isFavorite"
    />
  </div>
</template>
