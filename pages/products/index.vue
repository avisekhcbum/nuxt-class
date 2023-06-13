<template>
<div>
    <section class="py-5">
        <div class="container">
            <div class="row g-3">
                <div class="col-md-3" v-for="(product,index) in 30" :key="index">
                    <div class="card" style="width: 18rem;">
                        <div class="image-box">
                            <img src="https://cdn.pixabay.com/photo/2023/03/02/20/59/town-hall-tower-7826491__340.jpg" class="card-img-top" alt="...">
                        </div>
                        <div class="card-body">
                            <h5 class="card-title">Card title</h5>
                            <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                            <a href="#" class="btn btn-primary">Go somewhere</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</div>
</template>


<script setup>

</script>

<style  scoped>
img{
    filter: grayscale();
    transition: 1s;
}
img:hover{
    filter: none;
    transform: scale(2);
}
.image-box{
    overflow: hidden;
}
</style>
