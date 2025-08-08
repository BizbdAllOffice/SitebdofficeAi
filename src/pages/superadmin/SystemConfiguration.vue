<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="tabs">
        <button>General</button>
        <button>Timezone</button>
        <button>Currency</button>
        <button>Logo Upload</button>
      </div>
      <div class="tab-content">
        <!-- Tab Content Placeholder -->
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'SystemConfiguration',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.tabs { display: flex; gap: 1rem; margin-bottom: 1rem; }
.tab-content { background: #fff; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; }
</style>
