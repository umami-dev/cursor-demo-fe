<template>
  <div>
    <h1>Case 1</h1>
    <ul>
      <li v-for="(fruit, key) in fruits" :key="key">
        {{ fruit.name }} {{ fruit.emoji }}
      </li>
    </ul>
  </div>
</template>

<script setup>
const fruits = {
  apple: { name: 'Apple', emoji: '🍎' },
  banana: { name: 'Banana', emoji: '🍌' },
  cherry: { name: 'Cherry', emoji: '🍒' },
  elderberry: { name: 'Elderberry', emoji: '🫐' },
  fig: { name: 'Fig', emoji: '🧃' },
  grape: { name: 'Grape', emoji: '🍇' },
  kiwi: { name: 'Kiwi', emoji: '🥝' },
  lemon: { name: 'Lemon', emoji: '🍋' },
  mango: { name: 'Mango', emoji: '🥭' },
  nectarine: { name: 'Nectarine', emoji: '🍑' },
  orange: { name: 'Orange', emoji: '🍊' },
  pineapple: { name: 'Pineapple', emoji: '🍍' },
  strawberry: { name: 'Strawberry', emoji: '🍓' }
}
</script>
