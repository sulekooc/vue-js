<template>
  <div class="cart-item-card">
    <h3>Toplam Tutar : ${{ cart_total.toFixed(2) }}</h3>
    <button class="view-product-button">Ödeme Yapınız</button>
  </div>
</template>
<script>
export default {
  computed: {
    cart_total() {
      return this.$store.getters.cartTotal;
    },
  },
};
</script>