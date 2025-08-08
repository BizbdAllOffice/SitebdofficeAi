<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="dashboard-header">
        <h2>Dashboard Overview</h2>
        <input type="date" />
      </div>
      <div class="dashboard-cards">
        <div class="card">Users</div>
        <div class="card">Sales</div>
        <div class="card">Revenue</div>
        <div class="card">System Status</div>
      </div>
      <div class="dashboard-graphs">
        <!-- Graphs/Charts Placeholder -->
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'DashboardOverview',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.dashboard-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 1rem; }
.dashboard-cards { display: flex; gap: 1rem; margin-bottom: 2rem; }
.card { background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; flex: 1; text-align: center; }
.dashboard-graphs { min-height: 200px; background: #f9f9f9; border-radius: 8px; }
</style>
