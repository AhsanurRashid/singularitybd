<template>
    <div class="topnftcard_container">
        <div class="topnftcard_row">
            <div class="topnftcard_col">
                <div class="flex items-center gap-[22px]">
                    <div class="nft_id">{{ topNft?.id }}</div>
                    <div class="relative">
                        <img :src="require('@/assets/images/' + topNft?.image + '')" alt="owner_one">
                        <img v-if="topNft?.varified" class="verify_img" src="@/assets/images/verify.png" alt="verify">
                    </div>
                    <div>
                        <h3 class="nft_name">{{ topNft?.name }}</h3>
                        <div class="flex items-center gap-[6px]">
                            <img src="@/assets/images/ethereum.png" alt="ethereum">
                            <p class="nft_ethereum">{{ topNft?.ethereum }}</p>
                        </div>
                    </div>
                </div>
                <div class="nft_performance" :class="topNft?.status === 'good' ? 'text-[#14C8B0]' : 'text-[#FF002E]'">
                    +{{ topNft?.performance }}%
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ['topNft']
}
</script>

<style scoped>
    .topnftcard_row{
        @apply py-[16px];
    }
    .topnftcard_col {
        @apply flex items-center justify-between;
    }
    .nft_id {
        @apply font-[700] text-[24px] leading-[103%] tracking-[-0.025em] text-main;
    }
    .nft_name {
        @apply font-[500] text-[16px] leading-[103%] tracking-[-0.025em] text-main mb-[10px];     
    }
    .nft_ethereum {
        @apply font-[600] text-[14px] leading-[103%] tracking-[-0.025em] text-[#636363];     
    }
    .nft_performance {
        @apply font-[600] text-[20px] leading-[103%] tracking-[-0.025em];     
    }
    .verify_img {
        @apply absolute top-[-8px] right-[-8px];
    }
</style>