<template>
    <section id="topnftcollection_section">
        <div class="topnftcollection_container">
            <div class="topnftcollection_row">
                <div class="topnftcollection_col">
                    <div>
                        <img src="~/assets/images/top_main_img.png" alt="top_main_img">
                        <div class="owner_ethereum">
                            <div class="owner">
                                <img src="~/assets/images/e_owner.png" alt="e_owner">
                                <div>
                                    <h3>The Futr Abstr</h3>
                                    <p>10 in the stock</p>
                                </div>
                            </div>
                            <div class="ethereum_img">
                                <h4>Highest Bid</h4>
                                <div class="ethereum">
                                    <img src="~/assets/images/ethereum.png" alt="ethereum">
                                    <p>0.25 ETH</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="topnftcollection_col">
                    <div>
                        <NftownerCardVue  image_url="owner_one.png"/>
                        <NftownerCardVue image_url="owner_two.png"/>
                        <NftownerCardVue image_url="owner_three.png"/> 
                    </div>
                </div>
                <div class="topnftcollection_col">
                    <div class="top_collections">
                        <h1 class="">Top Collections over </h1>
                        <p class="">Last 7 days</p>
                        <div class="border-b border-[#F0F0F0] last:border-none" v-for="(topCollection, index) in topCollections" :key="`nft_${index}`">
                            <TopnftCard :topNft="topCollection"/>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import NftownerCardVue from '~/components/Global/NftownerCard.vue';
import TopnftCard from '../../Global/TopnftCard.vue';
export default {
    components: { NftownerCardVue, TopnftCard },
    data(){
        return {
            topCollections: [
                {
                    id: 1,
                    image: 'top_one.png',
                    name: 'CryptoFunks',
                    ethereum: '19,769.39',
                    performance: 26.52,
                    status: 'good',
                    varified: true
                },
                {
                    id: 2,
                    image: 'top_two.png',
                    name: 'Cryptix',
                    ethereum: '2,769.39',
                    performance: 10.52,
                    status: 'bad',
                    varified: false
                },
                {
                    id: 3,
                    image: 'top_three.png',
                    name: 'Frensware',
                    ethereum: '9,232.39',
                    performance: 2.52,
                    status: 'good',
                    varified: false
                },
                {
                    id: 4,
                    image: 'top_four.png',
                    name: 'PunkArt',
                    ethereum: '3,769.39',
                    performance: 1.52,
                    status: 'good',
                    varified: true
                },
                {
                    id: 5,
                    image: 'top_five.png',
                    name: 'Art Crypto',
                    ethereum: '10,769.39',
                    performance: 2.52,
                    status: 'bad',
                    varified: false
                }
            ]
        }
    }
}
</script>

<style scoped>
    #topnftcollection_section {
        @apply py-[134px];
    }
    .topnftcollection_container {
        @apply container mx-auto;
    }
    .topnftcollection_row {
        @apply grid grid-cols-3 gap-[53px];
    }
    .topnftcollection_col {

    }
    .owner_ethereum {
        @apply flex items-center justify-between py-[32px];
    }
    .owner {
        @apply flex items-center gap-[10px];
    }
    .owner h3{
        @apply font-[700] text-[20px] leading-[26px] text-main mb-[4px];
    }
    .owner p{
        @apply font-[400] text-[14px] leading-[18px] text-[#363639];
    }
    .ethereum_img h4 {
        @apply font-[500] text-[12px] leading-[16px] text-[#3A3A3A] mb-[7.18px];
    }
    .ethereum {
        @apply flex items-center gap-[10px];
    }
    .ethereum p {
        @apply font-[700] text-[16px] leading-[21px] text-[#3A3A3A];
    }

    .top_collections {
        @apply border-l border-[#ECECEC] pl-[30px];
    }
    .top_collections h1 {
        @apply font-[700] text-[20px] leading-[24px] text-main uppercase mb-[10px];
    }
    .top_collections p {
        @apply font-[700] text-[18px] leading-[32px] text-primary;
    }
</style>