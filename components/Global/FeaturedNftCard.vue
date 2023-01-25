<template>
    <div>
        <div class="featured_wrapper">
            <div class="featured_main_img">
                <img :src="require('@/assets/images/' + mainImg + '')" alt="f_nft_one">
            </div>
            <div class="featured_sub_images">
                <img src="@/assets/images/f_n_1_1.png" alt="f_n_1_1">
                <img src="@/assets/images/f_n_1_2.png" alt="f_n_1_2">
                <img src="@/assets/images/f_n_1_3.png" alt="f_n_1_3">
            </div>
        </div>
        <div class="featured_bottom">
            <h3>Amazing Collection</h3>
            <div class="flex items-center justify-between">
                <div class="flex items-center gap-[10px]">
                    <img src="@/assets/images/e_owner.png" alt="e_owner">
                    <p>by Arkhan</p>
                </div>
                <div class="total">Total 54 Items</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ['mainImg']
}
</script>

<style scoped>
    .featured_wrapper {
        @apply flex items-start gap-[8.25px];
    }   
    .featured_main_img img{
        @apply bg-[#C4C4C4] w-[295px] h-[272.27px] cursor-pointer rounded-[24px];
    }
    .featured_sub_images img {
        @apply bg-[#C4C4C4] w-[103.59px] h-[85.26px] rounded-[11.0008px] mb-[8.25px] last:mb-0 cursor-pointer;
    }
    .featured_bottom {
        @apply py-[30px];
    }
    .featured_bottom h3{
        @apply font-[700] text-[20px] leading-[26px] text-main mb-[10.4px] cursor-pointer;  
    }
    .featured_bottom p{
        @apply font-[500] text-[14px] leading-[18px] text-main cursor-pointer;  
    }
    .featured_bottom img {
        @apply w-[28px] h-[28px] cursor-pointer; 
    }
    .featured_bottom .total {
        @apply font-[700] text-[11.0008px] leading-[14px] text-primary border-2 border-primary py-[10px] px-[20px] rounded-[60px] inline-block cursor-pointer;
    }
</style>