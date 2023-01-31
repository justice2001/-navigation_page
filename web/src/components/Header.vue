<template>
  <div id="header">
    <div class="welcome">
      <div class="welcome-1">晚上好</div>
      <div class="welcome-2">欢迎访问正义的服务导航页面</div>
    </div>

    <div class="f1"></div>

    <div class="user">
      <img class="user-avatar" src="/icons/default.png" alt="Avatar">
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
#header {
  display: flex;
  align-items: center;
  margin: 45px;
}

.welcome-1 {
  font-size: 64px;
}

.welcome-2 {
  font-size: 32px;
}

.user-avatar {
  width: 120px;
  height: 120px;
  border-radius: 20px;
  background-color: #999;
}
</style>