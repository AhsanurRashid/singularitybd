<template>
  <div class="nftcard_wrapper">
    <div class="relative">
        <img class="w-full h-[222.7px] cursor-pointer bg-gray-200" src="@/assets/images/card_img.png" alt="card_img">
        <div class="nft_owners">
            <img src="@/assets/images/card_one.png" alt="card_img">
            <img class="ml-[-10px]" src="@/assets/images/card_two.png" alt="card_img">
            <img class="ml-[-10px]" src="@/assets/images/card_three.png" alt="card_img">
            <img class="ml-[-10px]" src="@/assets/images/card_four.png" alt="card_img">
        </div>
    </div>
    <div class="nftcard_caption">
        <h1>ArtCrypto</h1>
        <div class="flex items-center justify-between">
            <div class="flex items-center gap-[6px]">
                <img src="@/assets/images/green_ethereum.png" alt="ethereum">
                <p class="nft_ethereum">0.25 ETH</p>
            </div>
            <div class="ethereum_number">1 of 321</div>
        </div>
    </div>
    <div class="nftcard_bottom">
        <div class="left">3h 50m 2s left</div>
        <div class="right">Place a bid</div>
    </div>    
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .nftcard_wrapper {
        @apply bg-white rounded-[13.1647px] p-[11px];
    }
    .nft_owners {
        @apply absolute left-[12px] bottom-[-14px] flex items-center;
    }
    .nft_owners img {
        @apply bg-white p-[0.5px] rounded-full cursor-pointer;
    }
    .nftcard_caption {
        @apply pt-[22px] pb-[19.75px] border-b border-[#F4F4F4];
    }
    .nftcard_caption h1 {
        @apply font-[700] text-[19.7471px] leading-[19px] text-main mb-[10.72px] cursor-pointer;
    }
    .ethereum_number {
        @apply font-[500] text-[13.1647px] leading-[19px] text-[#838383];     
    }
    .nft_ethereum {
        @apply font-[700] text-[10.9706px] leading-[14px] text-[#00AC4F];     
    }
    .nftcard_bottom {
        @apply flex items-center justify-between py-[10.84px];
    }
    .nftcard_bottom .left {
        @apply inline-block font-light text-[10.9706px] leading-[19px] text-primary bg-[#F5F5F5] px-[20px] py-[10px] rounded-[109.706px] cursor-pointer;  
    }
    .nftcard_bottom .right {
        @apply inline-block font-[500] text-[15.3588px] leading-[20px] text-primary hover:bg-primary hover:text-white px-[20px] py-[10px] rounded-[109.706px] cursor-pointer transition-all ease-in-out duration-75 delay-75;  
    }
</style>