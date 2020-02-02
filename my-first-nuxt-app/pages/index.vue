<template>
  <div class="container">
    <Header />
    <nuxt-link to="users">Users</nuxt-link>
    <button @click="onProductsClick">Products</button>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Header from '~/components/Header.vue'

export default {
  components: {
    Logo, Header
  },
  methods: {
    onProductsClick(){
      this.$router.push('/products')
    }
  }
}
</script>

