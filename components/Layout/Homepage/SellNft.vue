<template>
  <section id="sellnft_section">
    <div class="sellnft_container">
        <div class="sellnft_row">
            <div class="sellnft_col_one">
                <div class="flex items-end flex-col gap-[52px]">
                    <div class="relative">
                       <img src="@/assets/images/sell_one.png" alt="sell_owner_one"> 
                       <img class="absolute right-[-35px] bottom-[-35px]" src="@/assets/images/sell_owner_one.png" alt="sell_owner_one"> 
                    </div>
                    <div class="relative">
                       <img src="@/assets/images/sell_two.png" alt="sell_owner_one"> 
                       <img class="absolute right-[-35px] bottom-[-35px]" src="@/assets/images/sell_owner_two.png" alt="sell_owner_one"> 
                    </div>
                </div>
                <div>
                    <div class="relative">
                       <img src="@/assets/images/sell_three.png" alt="sell_owner_one"> 
                       <img class="absolute right-[-35px] bottom-[-35px]" src="@/assets/images/sell_owner_two.png" alt="sell_owner_one"> 
                    </div>
                </div>
            </div>
            <div class="sellnft_col_two">
                <div>
                    <h1>Create and sell your NFTs</h1>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Facilisi ac phasellus placerat a pellentesque tellus sed egestas. Et tristique dictum sit tristique sed non. Lacinia lorem id consectetur pretium diam ut. Pellentesque eu sit blandit fringilla risus faucibus.</p>
                    <div class="btn">Sign Up Now</div>
                </div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
    #sellnft_section {
        @apply py-[102px];
    }
    .sellnft_container {
        @apply container mx-auto;
    }
    .sellnft_row {
        @apply grid grid-cols-2 gap-[78px];
    }
    .sellnft_col_one {
        @apply flex items-center justify-between;
    }
    .sellnft_col_two {
        @apply flex items-center;
    }
    .sellnft_col_two h1 {
        @apply w-[49%] font-[700] text-[32px] leading-[38px] text-main mb-[40px] uppercase;
    }
    .sellnft_col_two p {
        @apply w-[83%] font-light text-[18px] leading-[160%] text-[#636363] mb-[32px];
    }
    .sellnft_col_two .btn {
        @apply inline-block font-[400] text-[20px] leading-[25px] tracking-[0.065em] text-[#FFFFFF] bg-primary py-[18px] px-[40px] rounded-[60px] cursor-pointer;
    }
</style>