<template>
<div>
    <div class="container">
        <div class="row">
            <div class="col-md-4">
                <img :src="product.images[0]" alt="" class="img-fluid">
            </div>
            <div>
                <h1>{{ product.title }}</h1>
            </div>
            <div>
                <p>{{ product.description }}</p>
            </div>
            <div>
                <p>${{ product.price }}</p>
            </div>
        </div>
        <div>
            <h6>Category</h6>
            <p>{{ product.category.name }}</p>
            <img :src="product.category.image" alt="" width="80" class="rounded">
        </div>
        <div>
            <span><i class="fa-solid fa-circle-minus fs-1"></i></span>
            <span class="fs-1 px-5"></span>
            <span><i class="fa-solid fa-circle-plus fs-1"></i></span>
        </div>
    </div>
</div>
</template>

<script setup>
const route = useRoute();
const {data:product} =await useFetch(`https://api.escuelajs.co/api/v1/products/${route.params.id}`);
</script>

<style scoped>

</style>
