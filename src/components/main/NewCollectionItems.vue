<template>
    <section class="new-collection">
        <div class="container">
            <h3 class="text-capitalize">new collection</h3>
            <ul class="row list-unstyled g-4 mb-5">
                <li class="col-12 col-l-5 ">
                    <div class="d-flex flex-column">
                        <div class="jacket-collection position-relative m-1">
                            <p class="text-capitalize">Men’s Jacket Collection</p>
                            <picture>
                                <source srcset="@/assets/images/men-jeans-coat.png"  media="(min-width:770px">
                                <source srcset="@/assets/images/men-jeans-coat-sm.png" >
                                <img src="@/assets/images/men-jeans-coat-sm.png" alt="men-with-helmet">
                            </picture>
                            <router-link class="btn btn-black" to="#" title="discover">Discover Now</router-link>
                        </div>
                    </div>
                </li>
                <li class="col-12 col-l-7 ">
                    <div class="sunglasses-collection d-flex position-relative">
                        <picture class="col-6 col-md-7 col-l-7 col-xl-7 col-xxl-7">
                            <source srcset="@/assets/images/men-tshirt.png"  media="(min-width:770px">
                            <source srcset="@/assets/images/men-tshirt-sm.png" >
                            <img src="@/assets/images/men-tshirt-sm.png" alt="men-with-helmet">
                        </picture>
                        <div class="col-6 col-md-5  col-l-5 col-xl-5 col-xxl-5">
                            <p class="body-p text-capitalize">Men’s Sunglasses Collection</p>
                            <span class="text-uppercase offer">40% off</span>
                            <router-link class="btn btn-black" to="#" title="discover">Discover Now</router-link>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </section>
</template>