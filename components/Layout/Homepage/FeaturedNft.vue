<template>
  <section id="featured_section">
    <div class="featured_container">
        <h1 class="title">Collection Featured NFTs</h1>
        <div class="featured_row">
            <div class="featured_col">
                <FeaturedNftCard mainImg="f_nft_one.png"/>
            </div>
            <div class="featured_col">
                <FeaturedNftCard mainImg="f_nft_two.png"/>
            </div>
            <div class="featured_col">
                <FeaturedNftCard mainImg="f_nft_three.png"/>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
import FeaturedNftCard from '@/components/Global/FeaturedNftCard.vue'
export default {
  components: { FeaturedNftCard },

}
</script>

<style scoped>
    #featured_section {
        background: rgba(217, 224, 236, 0.2);
        backdrop-filter: blur(25px);
    }
    .featured_container {
        @apply container mx-auto py-[65px];
    }
    .featured_container .title{
        @apply font-[700] text-[28px] leading-[34px] text-main mb-[55px] uppercase;
    }
    .featured_row {
        @apply grid grid-cols-3 gap-[31px];
    }   
    .featured_col {

    }
</style>