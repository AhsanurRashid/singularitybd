<template>
  <section id="nftownercard_section">
    <div class="nftownercard_container">
        <div class="nftownercard_row">
            <div class="nftownercard_img">
                <img :src="require('@/assets/images/' + image_url + '')" alt="f_nft_one">
            </div>
            <div class="nftownercard_info">
                <h1>The Futr Abstr</h1>
                <div class="flex items-center gap-[10px] mb-[16px]">
                    <img class="w-[34px] h-[34px]" src="~/assets/images/e_owner.png" alt="e_owner">
                    <div class="eth">
                        <img src="~/assets/images/green_ethereum.png" alt="green_ethereum">
                        <p>0.25 ETH</p>
                    </div>
                    <p>1 of 8</p>
                </div>
                <div class="btn">Place a bid</div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    props: {
        image_url: String
    }
}
</script>

<style scoped>
    #nftownercard_section {
        @apply mb-[41px] last:mb-0;
    }
    .nftownercard_row {
        @apply flex items-start gap-[20px];
    }
    .nftownercard_info {
        @apply mt-[6px];
    }
    .nftownercard_info h1 {
        @apply font-[700] text-[20px] leading-[26px] text-main mb-[9px];
    }
    .nftownercard_info .eth {
        @apply flex items-center gap-[5px] p-[8px] border border-[#00AC4F] rounded-[6px];
    }
    .nftownercard_info .eth p {
        @apply font-[700] text-[12px] leading-[16px] text-[#00AC4F];
    }
    .nftownercard_info p {
        @apply font-[400] text-[14px] leading-[18px] text-[#757575];
    }
    .nftownercard_info .btn {
        @apply inline-block font-[400] text-[14px] leading-[17px] text-primary hover:text-[#FFFFFF] px-[20px] py-[14px] rounded-[50px] border-2 border-primary bg-white hover:bg-primary transition-all ease-in-out duration-75 delay-75 cursor-pointer;
    }
</style>