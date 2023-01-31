<template>
<a :href="link" target="_blank" class="app" :title="desc">
  <img class="app-icon" :src="icon == '' ? '/icons/default.png' : icon" :alt="name">
  <div class="app-name">{{ name }}</div>
</a>
</template>

<script setup>
defineProps({
  icon: String,
  name: String,
  link: String,
  desc: String
})
</script>

<style scoped>
.app {
  display: flex;
  flex-direction: column;
  align-items: center;
  cursor: pointer;
}

.app:hover .app-icon {
  transform: scale(1.1);
}

.app:active .app-icon {
  transform: scale(0.9);
  filter: brightness(0.8);
}

.app-icon {
  width: 130px;
  height: 130px;
  border-radius: 20px;

  transition: transform .3s;
}

.app-name {
  font-size: 18px;
  margin-top: 10px;
  text-align: center;
}
</style>