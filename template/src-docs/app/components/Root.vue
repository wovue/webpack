<template>
  <div>
    <sidebar></sidebar>
    <router-view></router-view>
    <gh-corner v-transfer-dom repo-user="{{ repoUser }}" repo-name="{{ repoName }}" color="#EAE8EB" background="#dd5a6f"></gh-corner>
  </div>
</template>

<script>
  import GhCorner from './GhCorner'
  import Sidebar from './Sidebar'

  export default {
    name: 'Root',
    components: {
      GhCorner,
      Sidebar
    }
  }
</script>
