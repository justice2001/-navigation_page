<template>
  <div id="container">
    <Header />
    <div id="main">
      <AppList />
    </div>

    <div id="footer">
      <p>
        Copyright ©️ 2022-2023 正义OvO, All rights reserved! Source Code [
        <a class="sc-link" href="https://git.mczhengyi.top/zhengyi/navigation_page">Gitea</a>
        <a class="sc-link" href="#" title="暂不提供" style="text-decoration-line: line-through;">Github</a>
        <a class="sc-link" href="#" title="暂不提供" style="text-decoration-line: line-through;">码云仓库</a>
        ] (version 0.1a)
      </p>
    </div>
  </div>
</template>

<script setup>
import Header from "./components/Header.vue";
import AppList from "./components/AppList.vue";
</script>

<style scoped>
h1 {
  margin: 0;
}

#container {
  height: 100vh;
  display: flex;
  flex-direction: column;
}

#main {
  flex: 1;
  margin: 20px 45px 0 45px;
}

#footer {
  text-align: center;
}

.sc-link {
  margin: 0 5px;
}
</style>