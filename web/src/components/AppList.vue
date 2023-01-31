<template>
  <div class="app-list">
    <AppIns v-for="i in appList" :icon="i.icon"
            :name="i.name"
            :link="i.link"
            :desc="i.description" />
  </div>
</template>

<script setup>
import AppIns from "./app-list/AppIns.vue";

const countPerPage = 10;
const appList = [
  {id: 1, name: "Jellyseerr媒体管理", icon: '/icons/jellyseerr.png', link: "http://192.168.31.13:5055", description: "统一媒体管理平台", category: 1, pb: false},
  {id: 1, name: "QBittorent下载器", icon: '/icons/qbittorent.png', link: "http://192.168.31.13:8080", description: "BT下载软件", category: 1, pb: false},
  {id: 1, name: "Sonarr追剧/番", icon: '/icons/sonarr.png', link: "http://192.168.31.13:8989", description: "自动下载影片、追番", category: 1, pb: false},
  {id: 1, name: "Emby媒体库", icon: '/icons/emby.png', link: "http://192.168.31.13:8096", description: "媒体串流软件", category: 1, pb: false},
  {id: 1, name: "Gitea代码仓库", icon: '/icons/gitea.png', link: "https://git.mczhengyi.top", description: "媒体串流软件", category: 1, pb: true},
  {id: 1, name: "Exsi服务器", icon: '/icons/exsi.png', link: "http://192.168.31.2", description: "媒体串流软件", category: 1, pb: true},
  {id: 1, name: "VCenter管理平台", icon: '/icons/vcenter.png', link: "http://192.168.31.10", description: "媒体串流软件", category: 1, pb: true},
  {id: 1, name: "Blog-博客", icon: '/icons/typecho.png', link: "https://blog.mczhengyi.top", description: "媒体串流软件", category: 1, pb: true},
]
</script>

<style scoped>
.app-list {
  margin: 20px;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-gap: 20px;
}
</style>