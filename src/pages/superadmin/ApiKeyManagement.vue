<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="api-list">
        <div class="api-key">API Key 1 <button>Generate</button></div>
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'ApiKeyManagement',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.api-list { margin: 2rem 0; }
.api-key { background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; margin-bottom: 1rem; display: flex; justify-content: space-between; align-items: center; }
</style>
