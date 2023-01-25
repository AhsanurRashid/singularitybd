<template>
  <section id="hero_section">
    <div class="hero_container">
        <div class="hero_row">
            <div class="hero_col">
                <h1 class="hero_title">
                    Discover, and collect Digital Art  NFTs 
                </h1>
                <p class="hero_description">Digital marketplace for crypto collectibles and non-fungible tokens (NFTs). Buy, Sell, and discover exclusive digital assets.</p>
                <div class="hero_btn">Explore Now</div>
                <div class="hero_text_wrapper">
                    <div class="hero_text">
                        <h1>98k+</h1>
                        <p>Artwork</p>
                    </div>
                    <div class="hero_text">
                        <h1>12k+</h1>
                        <p>Auction</p>
                    </div>
                    <div class="hero_text">
                        <h1>15k+</h1>
                        <p>Artist</p>
                    </div>
                </div>
            </div>
            <div class="hero_col relative">
                <Slider/>
                <img class="live" src="~/assets/images/live.png" alt="live">
            </div>
        </div>
    </div>
    <img class="dot" src="@/assets/images/dot.png" alt="dot">
  </section>
</template>

<script>
    import Slider from '~/components/Global/Slider.vue';
    export default {
        components: { Slider }
    }
</script>

<style scoped>
    #hero_section {
        @apply py-[100px];
    }
    .dot {
      z-index: -1;
      @apply absolute left-[25px] bottom-[160px];
    }
    .live {
        @apply absolute bottom-[95px] left-[59px];
    }
    .hero_container {
        @apply container mx-auto;
    }
    .hero_row {
        @apply grid grid-cols-2;
    }
    .hero_col {

    }
    .hero_title {
        font-family: 'MyTitleFont', Fallback, sans-serif !important;
        @apply font-[700] text-[40px] leading-[48px] tracking-[0.05em] text-main uppercase mb-[22px];
    }
    .hero_description {
        @apply font-light text-[20px] leading-[160%] text-[#565656] mb-[41px] w-[71%];
    }
    .hero_btn {
        @apply inline-block cursor-pointer shadow px-[40px] py-[20px] bg-primary rounded-[60px] font-[400] text-[20px] leading-[25px] tracking-[0.065em] text-[#FFFFFF];
    }
    .hero_text_wrapper {
        @apply flex items-center gap-[23px] mt-[30px];
    }
    .hero_text h1 {
        @apply font-[700] text-[40px] leading-[48px] tracking-[0.05em] text-main;
    }
    .hero_text p {
        @apply font-light text-[20px] leading-[160%] text-[#565656] mt-[-5px];
    }

    .swiper {
  width: 240px;
  height: 320px;
}

.swiper-slide {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 18px;
  font-size: 22px;
  font-weight: bold;
  color: #fff;
}

.swiper-slide:nth-child(1n) {
  background-color: rgb(206, 17, 17);
}

.swiper-slide:nth-child(2n) {
  background-color: rgb(0, 140, 255);
}

.swiper-slide:nth-child(3n) {
  background-color: rgb(10, 184, 111);
}

.swiper-slide:nth-child(4n) {
  background-color: rgb(211, 122, 7);
}

.swiper-slide:nth-child(5n) {
  background-color: rgb(118, 163, 12);
}

.swiper-slide:nth-child(6n) {
  background-color: rgb(180, 10, 47);
}

.swiper-slide:nth-child(7n) {
  background-color: rgb(35, 99, 19);
}

.swiper-slide:nth-child(8n) {
  background-color: rgb(0, 68, 255);
}

.swiper-slide:nth-child(9n) {
  background-color: rgb(218, 12, 218);
}

.swiper-slide:nth-child(10n) {
  background-color: rgb(54, 94, 77);
}
</style>