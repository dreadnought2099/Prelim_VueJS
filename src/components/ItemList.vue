<script setup>
const handleAddToCart = (productName) => {
  console.log(`Product added to cart: ${productName}`);
};
</script>

<template>
  <div class="product-list">
    <h2>Product List</h2>
    <div class="product">
      <h3>Product 1</h3>
      <p>Price: $100</p>
      <button @click="handleAddToCart('Product 1')">Add to cart</button>
    </div>
    <div class="product">
      <h3>Product 2</h3>
      <p>Price: $69</p>
      <button @click="handleAddToCart('Product 2')">Add to cart</button>
    </div>
    <div class="product">
      <h3>Product 3</h3>

      <p>Price: $18</p>
      <button @click="handleAddToCart('Product 3')">Add to cart</button>
    </div>
  </div>
</template>

<style>
.product {
  margin-bottom: 30px;
}
</style>
