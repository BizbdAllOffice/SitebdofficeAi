<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="backup-actions">
        <button>Create Backup</button>
        <input type="file" />
        <button>Restore</button>
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'BackupRestore',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.backup-actions { display: flex; gap: 1rem; margin: 2rem 0; }
</style>
