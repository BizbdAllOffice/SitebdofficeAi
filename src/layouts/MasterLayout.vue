<template>
  <div>
    <Header />
    <main>
      <slot />
    </main>
    <Footer />
  </div>
</template>
<script>
import Header from '../components/Header.vue';
import Footer from '../components/Footer.vue';
export default {
  name: 'MasterLayout',
  components: { Header, Footer }
}
</script>
