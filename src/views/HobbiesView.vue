<template>
  <div class="hobbies">
    <div class="section">
        <h2>Quais são os meus Hobbies?</h2>
        <ul>
            <li v-for="(item, i) in list_hobbies" :key="i">{{ item }}</li>
        </ul>
    </div>
  </div>
</template>
<script setup>
  const list_hobbies = [
    "Cinema com a família",
    "Churrasco com os amigos",
    "Futebol aos finais de semana"
  ]
</script>
