<template>
  <SuperAdminLayout>
    <template v-slot:default>
      <form class="profile-form">
        <h2>Super Admin Profile</h2>
        <label>Name: <input type="text" /></label>
        <label>Email: <input type="email" /></label>
        <label>Password: <input type="password" /></label>
        <button type="submit">Update Profile</button>
      </form>
    </template>
  </SuperAdminLayout>
</template>
<script>
import SuperAdminLayout from '../../layouts/SuperAdminLayout.vue';
export default {
  name: 'SuperAdminProfile',
  components: { SuperAdminLayout }
}
</script>
<style scoped>
.profile-form { max-width: 400px; margin: 2rem auto; background: #fff; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 8px #eee; }
.profile-form label { display: block; margin-bottom: 1rem; }
</style>
