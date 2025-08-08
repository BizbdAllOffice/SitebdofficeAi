<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="header">
        <h2>User Management</h2>
        <input type="search" placeholder="Search users..." />
      </div>
      <table class="user-table">
        <thead>
          <tr><th>Name</th><th>Role</th><th>Status</th><th>Actions</th></tr>
        </thead>
        <tbody>
          <tr><td>John Doe</td><td>Admin</td><td>Active</td><td><button>Edit</button></td></tr>
        </tbody>
      </table>
      <div class="modal" v-if="showModal">
        <!-- Add/Edit User Modal -->
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'UserManagement',
  components: { SuperAdminLayout },
  data() {
    return { showModal: false };
  }
}
</script>
<style scoped>
.header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 1rem; }
.user-table { width: 100%; border-collapse: collapse; margin-bottom: 2rem; }
.user-table th, .user-table td { border: 1px solid #ddd; padding: 0.5rem; }
.modal { position: fixed; top: 20%; left: 50%; transform: translate(-50%, 0); background: #fff; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; }
</style>
