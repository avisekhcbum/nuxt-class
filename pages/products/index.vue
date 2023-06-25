<template>
<div>
    <div class="py-5">
        <div class="container">
            <div class="row g-4">
                <div class="col-md-4" v-for="(p,index) in product" :key="index">
                    <nuxt-link :to="`/products/${p.id}`" style="text-decoration:none;">
                        <productCard :product="p"/>
                    </nuxt-link>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script setup>
const {data:product} = await useFetch ("https://api.escuelajs.co/api/v1/products");
   
</script>

<style scoped>
img {
    filter: grayscale();
    transition: 1s;
}

img:hover {
    filter: none;
    transform: scale(2);
}

.image-box {
    overflow: hidden;
}
</style>
