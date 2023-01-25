<template>
  <div>
    <HeroSection/>
    <AmazingNft />
    <TopnftCollection />
    <FeaturedNft />
    <SellNft />
    <AlllNfts />
  </div>
</template>

<script>
import HeroSection from '~/components/Layout/Homepage/HeroSection.vue';
import AmazingNft from '~/components/Layout/Homepage/AmazingNft.vue';
import TopnftCollection from '~/components/Layout/Homepage/TopnftCollection.vue';
import FeaturedNft from '~/components/Layout/Homepage/FeaturedNft.vue';
import SellNft from '../components/Layout/Homepage/SellNft.vue';
import AlllNfts from '../components/Layout/Homepage/AlllNfts.vue';

export default {
    name: "IndexPage",
    head: {
        title: "NFT"
    },
    components: { HeroSection, AmazingNft, TopnftCollection, FeaturedNft, SellNft, AlllNfts }
}
</script>
