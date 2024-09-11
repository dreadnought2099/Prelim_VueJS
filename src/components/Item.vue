<template></template>

<script>
export default {
  name: "Item",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
  methods: {
    addToCart() {
      console.log(`Added to cart: ${this.item.name} - $${this.item.price}`);
      this.$emit("add-to-cart", this.item);
    },
  },
};
</script>
