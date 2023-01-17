
<template>
  <section>
    <header>
      <CoverItems/> 
    </header>
    <main>
      <ResponsiveNav/>
      <BrandsCooperation/>
      <NewCollection/>
      <BestSellers/>
    </main>
    <footer>
      <Footer/>
    </footer>
  </section>
</template>

<script>
import CoverItems from '@/components/header/CoverItems.vue'
import ResponsiveNav from '@/components/main/ResponsiveNavItems.vue'
import BrandsCooperation from '@/components/main/BrandsCooperation.vue'
import NewCollection from '@/components/main/NewCollectionItems.vue'
import BestSellers from '@/components/main/BestSellersItems.vue'
import Footer from '@/components/footer/Footer.vue'

export default {
  components: {
    CoverItems,
    ResponsiveNav,
    BrandsCooperation,
    NewCollection,
    BestSellers,
    Footer
  }
}
</script>
