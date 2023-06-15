<template>
<div>
    <h1>Product Detailed Page</h1>
    <h2>The product number is {{ route.params.id }}</h2>
</div>
</template>

<script setup>
const route = useRoute();
</script>

<style lang="scss" scoped>

</style>
