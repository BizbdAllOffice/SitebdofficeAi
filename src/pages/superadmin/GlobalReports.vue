<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="report-header">
        <input type="date" />
        <input type="date" />
      </div>
      <div class="report-graphs">
        <!-- Multiple Graphs Placeholder -->
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'GlobalReports',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.report-header { display: flex; gap: 1rem; margin-bottom: 1rem; }
.report-graphs { min-height: 200px; background: #f9f9f9; border-radius: 8px; }
</style>
