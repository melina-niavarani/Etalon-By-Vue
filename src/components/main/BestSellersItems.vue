<template>
    <section class="best-seller">
        <div class="container">
            <h3 class="text-capitalize">Best Sellers</h3>
            <ul class="row flex-nowrap list-unstyled overflow-auto">
                <li class="col">
                    <div class="card">
                        <span class="percent d-none d-md-block d-lg-none"></span>
                        <span class="icon icon-heart"></span>
                        <img class="product-img" src="@/assets/images/backpack.svg" alt="bagpack">
                    </div>
                    <div class="d-flex ">
                        <div class="col-10 position-relative">
                            <p class="sub ">Fjallraven Backpack</p>
                            <p><span class="price d-md-none d-lg-block mb-0 ">$109.95</span></p>
                            <p><span class="price new-price position-absolute d-none d-md-block d-lg-none" ><rubby class="opacity-25 text-decoration-line-through me-2">$157</rubby>$109.95</span></p>
                        </div>
                        <span class="cart new-pos align-self-center text-end col-1 position-relative" @click="increment" >
                            <img src="@/assets/images/plus.png" alt="plus" class="plus">
                            <img src="@/assets/images/cart-square.svg">
                        </span>
                    </div>
                </li>
                <li class="col">
                    <div class="card">
                        <span class="icon icon-heart"></span>
                        <img class="product-img" src="@/assets/images/beige-coat.svg" alt="beige-coat">
                    </div>
                    <div class="d-flex">
                        <div class="col-10">
                            <p class="sub">Mens Cotton Jacket</p>
                            <p><span class="price">$55.99</span></p>
                        </div>
                        <span class="cart align-self-center text-end col-1 position-relative" @click="increment">
                            <img src="@/assets/images/plus.png" alt="plus" class="plus">
                            <img src="@/assets/images/cart-square.svg">
                        </span>
                    </div>
                </li>
                <li class="col">
                    <div class="card">
                        <span class="icon icon-heart"></span>
                        <img class="product-img" src="@/assets/images/white-shirt.svg" alt="slim-fit-tshirt">
                    </div>
                    <div class="d-flex">
                        <div class="col-10">
                            <p class="sub">Slim Fit T-Shirts</p>
                            <p><span class="price">$22.3</span></p>
                        </div>
                        <span class="cart align-self-center text-end col-1 position-relative" @click="increment">
                            <img src="@/assets/images/plus.png" alt="plus" class="plus">
                            <img src="@/assets/images/cart-square.svg">
                        </span>
                    </div>
                </li>
                <li class="col">
                    <div class="card">
                        <span class="percent"></span>
                        <span class="icon icon-heart"></span>
                        <img class="product-img" src="@/assets/images/blue-shirt.svg" alt="casual-slim-fit">
                    </div>
                    <div class="d-flex">
                        <div class="col-10">
                            <p class="sub">Mens Casual Slim Fit</p>
                            <p><span class="price"><rubby class="opacity-25 text-decoration-line-through me-2">$15.99</rubby>$11.25</span></p>
                        </div>
                        <span class="cart align-self-center text-end col-1 position-relative" @click="increment">
                            <img src="@/assets/images/plus.png" alt="plus" class="plus">
                            <img src="@/assets/images/cart-square.svg">
                        </span>
                    </div>
                </li>
            </ul>
        </div>
        <div class="text-center pb-5 d-none d-lg-block">
            <router-link class="btn btn-black2"  to="#" title="more-product"> Load More Products</router-link>
        </div>
    </section>
</template>

<script>
    import { mapActions, mapStores } from 'pinia';
    import { useCounterStore } from '@/stores/counter'

    export default {
    computed: {
        ...mapStores(useCounterStore)
    } ,
    methods: {
        ...mapActions(useCounterStore, ['increment'])
    }
    }
</script>