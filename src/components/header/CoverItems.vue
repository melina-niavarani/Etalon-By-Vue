<template>
    <div class="cover">
        <div class="container">
            <div class="row justify-content-center">
                <div class="cover-details col-12 col-l-5 col-xl-5 col-xxl-5">
                    <span>2022</span>
                    <h1>Autumn Jackets</h1>
                    <h4>Autumn Sale/ Up to 50% OFF</h4>
                    <a class="btn btn-yellow text-capitalize">open collection</a>
                </div>
                <div class="col-12 col-md-12 col-l-6 col-xl-6 col-xxl-6 position-relative">
                    <div class="d-xxl-block d-xl-block d-l-block d-md-block d-none">
                        <img class="layer1 position-absolute" src="@/assets/images/circle-layer.svg" alt="circle-layer">
                        <img class=" layer2 position-absolute" src="@/assets/images/circle-layer.svg" alt="circle-layer">
                    </div>
                    <p id="cover-price" class="position-absolute d-none d-lg-block d-xl-block d-xxl-block">$299</p>
                    <div class="d-none d-xl-block d-xxl-block">
                        <span class="flash1 icon-flash-left"></span>
                        <span class="flash2 icon-flash-right"></span>
                    </div>
                    <picture class="cover-img position-relative " >
                        <source srcset="@/assets/images/men-with-helmet.png "  media="(min-width:768px)">
                        <source srcset="@/assets/images/Group2.svg" >
                        <img src="@/assets/images/Group2.svg" alt="men-with-helmet">
                    </picture>
                    <img class="off position-absolute d-none d-lg-block d-xl-block d-xxl-block" src="../../assets/images/off.svg" alt="%off">
                </div>
                <div class="circles position-relative col-12 col-l-1 col-xl-1 col-xxl-1 m-auto">
                    <router-link to="#"><div class="circle1"></div></router-link>
                    <router-link to="#"><div class="circle2"></div></router-link>
                    <router-link to="#"><div class="circle3"></div></router-link>
                </div>
            </div>
        </div>
    </div>
</template>