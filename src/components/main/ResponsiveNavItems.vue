<template>
    <nav class="img-navbar d-lg-none d-xl-none d-xxl-none ">
        <div class="container">
            <ul class="d-flex justify-content-between align-content-center list-unstyled">
                <li>
                    <router-link  :to="{
                            name: 'contact',
                            query: {
                                name: 'contact-us',
                                value: 'bar'
                            }
                        } " ><img src="@/assets/images/phone.svg" alt="phone"></router-link>
                </li>
                <li>
                    <router-link to=""><img src="@/assets/images/tag.svg" alt="tag"></router-link>
                </li>
                <li>
                    <router-link :to="{
                            name: 'home',
                            query: {
                                name: 'home',
                                value: '100?'
                            }
                        } "><img src="@/assets/images/home.svg" alt="home"></router-link>
                </li>
                <li>
                    <router-link to=""><img src="@/assets/images/store.svg" alt="store"></router-link>
                </li>
                <li class="cart-container">
                    <span class="counter">{{ counterStore.count }}</span> 
                    <router-link to=""><img src="@/assets/images/cart1.svg" alt="cart"></router-link>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
import { useCounterStore } from '@/stores/counter';
import { mapStores } from 'pinia';

export default {
    computed: {
        ...mapStores(useCounterStore)
    }
}
</script>