<template>
<div>
    <div class="py-5">
        <div class="container">
            <div class="row g-4">
                <div class="col-md-3" v-for="(p, index) in product" :key="index">
                    <productCard :product="p" />
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
const {data: product} = await useFetch("https://api.escuelajs.co/api/v1/products");
console.warn(data.data._rawValue);
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
