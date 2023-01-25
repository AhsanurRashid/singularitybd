<template>
  <section id="allnft_section">
    <div class="allnft_container">
        <div class="allnft_row_one">
            <h1>Discover more NFTs</h1>
            <div class="tabs">
                <div @click="handleClick(tab)" v-for="(tab, index) in tabs" :key="`tabs_${index}`" class="tab" :class="tabId === tab?.id ? 'text-white bg-primary' : 'text-main bg-gray-100'">
                    <div>{{ tab.name }}</div>
                </div>
            </div>
        </div>
        <div v-if="!loading" class="allnft_row_two">
            <div v-for="n in 16" :key="n">
                <NftCard />
            </div>
        </div>
        <div v-else class="w-full h-[250px] flex items-center justify-center bg-white rounded-[10px]">
            <svg width="50px" height="50px"  xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 100 100" preserveAspectRatio="xMidYMid" style="background: none;">
                <circle cx="75" cy="50" fill="#363a3c" r="6.39718">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="-0.875s"></animate>
                </circle>
                <circle cx="67.678" cy="67.678" fill="#363a3c" r="4.8">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="-0.75s"></animate>
                </circle>
                <circle cx="50" cy="75" fill="#363a3c" r="4.8">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="-0.625s"></animate>
                </circle>
                <circle cx="32.322" cy="67.678" fill="#363a3c" r="4.8">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="-0.5s"></animate>
                </circle>
                <circle cx="25" cy="50" fill="#363a3c" r="4.8">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="-0.375s"></animate>
                </circle>
                <circle cx="32.322" cy="32.322" fill="#363a3c" r="4.80282">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="-0.25s"></animate>
                </circle>
                <circle cx="50" cy="25" fill="#363a3c" r="6.40282">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="-0.125s"></animate>
                </circle>
                <circle cx="67.678" cy="32.322" fill="#363a3c" r="7.99718">
                    <animate attributeName="r" values="4.8;4.8;8;4.8;4.8" times="0;0.1;0.2;0.3;1" dur="1s" repeatCount="indefinite" begin="0s"></animate>
                </circle>
            </svg>
        </div>
    </div>
  </section>
</template>

<script>
import NftCard from '../../Global/NftCard.vue'
export default {
  components: { NftCard },
    data(){
        return {
            tabId : 1,
            loading: false,
            tabs: [
                {
                    id: 1,
                    name: 'All Categories'
                },
                {
                    id: 2,
                    name: 'Art'
                },
                {
                    id: 3,
                    name: 'Celebrities'
                },
                {
                    id: 4,
                    name: 'Gaming'
                },
                {
                    id: 5,
                    name: 'Sport'
                },
                {
                    id: 6,
                    name: 'Music'
                },
                {
                    id: 7,
                    name: 'Crypto'
                }
            ]
        }
    },
    methods: {
        handleClick(tab){
            this.tabId = tab.id
            this.loading = true
            setTimeout(()=>{
                this.loading = false
            }, 2000)
        }
    }
}
</script>

<style scoped>
    #allnft_section {
        background: rgba(217, 224, 236, 0.2);
        backdrop-filter: blur(25px);
        @apply py-[64px];
    }
    .allnft_container {
        @apply container mx-auto;
    }
    .allnft_row_one .tabs{
        @apply flex items-center gap-[12px] mb-[40px];
    }
    .allnft_row_one .tab{
        @apply font-[500] text-[14px] leading-[17px] px-[20px] py-[10px] hover:text-white hover:bg-primary rounded-[100px] cursor-pointer transition-all ease-in-out duration-75 delay-75;
    }
    .allnft_row_one h1 {
        @apply font-[700] text-[34px] leading-[41px] text-main mb-[36px] uppercase;
    }
    .allnft_row_two {
        @apply grid grid-cols-4 gap-[39.49px];
    }
</style>