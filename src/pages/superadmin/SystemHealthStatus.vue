<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="status-cards">
        <div class="card">Server Status <div class="progress"><div class="bar" style="width:80%"></div></div></div>
        <div class="card">App Status <div class="progress"><div class="bar" style="width:95%"></div></div></div>
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'SystemHealthStatus',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.status-cards { display: flex; gap: 1rem; }
.card { background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; flex: 1; }
.progress { background: #eee; height: 10px; border-radius: 5px; margin-top: 1rem; }
.bar { background: #4caf50; height: 100%; border-radius: 5px; }
</style>
