<script setup>
import Card from './Card.vue'
</script>

const onclickAdd = () => { alert("Add!") }

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      title="Мужские Кроссовки Nike Blazer Mid Suede"
      :price="5000"
      imageUrl="/sneakers/sneakers-1.jpg"
      :isFavorite="false"
      :onclickAdd="onclickAdd"
    />
  </div>
</template>
