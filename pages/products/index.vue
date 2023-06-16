<template>
<div>
    <div class="py-5">
        <div class="container">
            <div class="row g-3">
                <div class="col-md-3" v-for="(product,index) in 30" :key="index">
                    <productCard></productCard>
                </div>
            </div>
        </div>
</div>
</div>
</template>

<script>
import { dataToEsm } from '@rollup/pluginutils';

const {data} = await useFetch("https://api.escuelajs.co/api/v1/products")
console.warn(data)
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
