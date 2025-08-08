<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="plan-list">
        <div class="plan">Basic Plan <button>Edit</button></div>
      </div>
      <div class="modal" v-if="showModal">
        <!-- Add/Edit Plan Modal -->
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'SubscriptionManagement',
  components: { SuperAdminLayout },
  data() {
    return { showModal: false };
  }
}
</script>
<style scoped>
.plan-list { margin: 2rem 0; }
.plan { background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; margin-bottom: 1rem; display: flex; justify-content: space-between; align-items: center; }
.modal { position: fixed; top: 20%; left: 50%; transform: translate(-50%, 0); background: #fff; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; }
</style>
