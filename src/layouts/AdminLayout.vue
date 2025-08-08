<template>
  <div>
    <Header />
    <Sidebar />
    <main>
      <slot />
    </main>
    <Footer />
  </div>
</template>
<script>
import Header from '../components/Header.vue';
import Sidebar from '../components/Sidebar.vue';
import Footer from '../components/Footer.vue';
export default {
  name: 'AdminLayout',
  components: { Header, Sidebar, Footer }
}
</script>
