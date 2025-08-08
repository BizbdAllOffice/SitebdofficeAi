<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <table class="audit-table">
        <thead>
          <tr><th>Date</th><th>User</th><th>Action</th><th>IP</th></tr>
        </thead>
        <tbody>
          <tr><td>2025-08-08</td><td>Admin</td><td>Login</td><td>192.168.1.1</td></tr>
        </tbody>
      </table>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'AuditLogViewer',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.audit-table { width: 100%; border-collapse: collapse; }
.audit-table th, .audit-table td { border: 1px solid #ddd; padding: 0.5rem; }
</style>
