<template>
    <div>
        <div class="navbar navbar-expand-lg navbar-dark d-none d-lg-block">
            <div class="container">
                <router-link id="brand" class="navbar-brand" to="#Etalon" title="etalon">Etalon</router-link>
                <div>
                    <ul class="navbar-nav"> 
                        <li class="nav-item ">
                            <router-link class="nav-link " 
                            :to="{
                                name: 'home',
                                query: {
                                    name: 'home',
                                    value: '100?'
                                }
                            } "  title="home">Home</router-link>
                        </li>
                        <li class="nav-item ">
                            <router-link class="nav-link " to="#store" title="store">store</router-link>
                        </li>
                        <li class="nav-item ">
                            <router-link class="nav-link" to="#new" title="new">New</router-link>
                        </li>
                        <li class="nav-item ">
                            <router-link class="nav-link " 
                            :to="{
                                name: 'contact',
                                query: {
                                    name: 'contact-us',
                                    value: 'bar'
                                }
                            } " 
                            title="contact">Contact</router-link>
                        </li>
                    </ul>
                </div>
                <div class="cart-container">
                    <span class="counter">{{ counterStore.count }}</span> 
                    <img id="cart" src="@/assets/images/cart.svg" alt="cart-img">
                </div> 
            </div>
        </div>
    </div>
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

