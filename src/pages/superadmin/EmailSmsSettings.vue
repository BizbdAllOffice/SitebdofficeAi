<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="tabs">
        <button>Email Templates</button>
        <button>SMS Templates</button>
      </div>
      <div class="tab-content">
        <!-- Email/SMS Template Content -->
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'EmailSmsSettings',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.tabs { display: flex; gap: 1rem; margin-bottom: 1rem; }
.tab-content { background: #fff; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; }
</style>
