<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <form class="role-form">
        <h2>Role & Permission Settings</h2>
        <label>Role Name: <input type="text" /></label>
        <div class="permissions">
          <label><input type="checkbox" /> Read</label>
          <label><input type="checkbox" /> Write</label>
          <label><input type="checkbox" /> Delete</label>
        </div>
        <button type="submit">Save/Update</button>
      </form>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'RolePermissionSettings',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.role-form { max-width: 400px; margin: 2rem auto; background: #fff; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; }
.permissions { display: flex; gap: 1rem; margin: 1rem 0; }
</style>
