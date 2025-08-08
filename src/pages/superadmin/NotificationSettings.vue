<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="notification-list">
        <label><input type="checkbox" /> Email Notification</label>
        <label><input type="checkbox" /> SMS Notification</label>
        <label><input type="checkbox" /> Push Notification</label>
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'NotificationSettings',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.notification-list { display: flex; flex-direction: column; gap: 1rem; margin: 2rem 0; }
</style>
