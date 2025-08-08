<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <div class="payment-cards">
        <div class="card">Stripe <input type="text" placeholder="API Key" /></div>
        <div class="card">PayPal <input type="text" placeholder="API Key" /></div>
        <div class="card">SSLCommerz <input type="text" placeholder="API Key" /></div>
      </div>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'PaymentGatewaySettings',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.payment-cards { display: flex; gap: 1rem; }
.card { background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; flex: 1; }
</style>
