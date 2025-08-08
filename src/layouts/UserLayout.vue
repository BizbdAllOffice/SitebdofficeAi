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
  name: 'UserLayout',
  components: { Header, Footer }
}
</script>
