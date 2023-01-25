<template>
    <div class="">
        <section id="slider">
            <input class="card-slider" type="radio" name="slider" id="s3" checked>
            <input class="card-slider" type="radio" name="slider" id="s4">
            <input class="card-slider" type="radio" name="slider" id="s5">
            <label for="s3" id="slide3" class="card-slider relative">
                <img class="card_image" src="~/assets/images/one.png" alt="one">
                <div class="card_caption_one">
                    <div class="caption_title">Abstr Gradient NFT</div>
                    <div class="caption_owner">
                        <img src="~/assets/images/owner.png" alt="owner">
                        <p>Arkhan17</p>
                    </div>
                </div>
                <div class="card_caption_two">
                    <div class="card_count_wrapper">
                        <p class="title">Current Bid</p>
                        <div class="card_count">
                            <img src="~/assets/images/eth.png" alt="eth">
                            <p>0.25 ETH</p>
                        </div>
                    </div>
                    <div class="card_count_wrapper">
                        <p class="title">Ends in</p>
                        <div class="card_count">
                            <p>12h  43m  42s</p>
                        </div>
                    </div>
                </div>
            </label>
            <label for="s4" id="slide4" class="card-slider relative">
                <img class="card_image" src="~/assets/images/two.png" alt="one">
                <div class="card_caption_one">
                    <div class="caption_title">Abstr Gradient NFT</div>
                    <div class="caption_owner">
                        <img src="~/assets/images/owner.png" alt="owner">
                        <p>Arkhan17</p>
                    </div>
                </div>
                <div class="card_caption_two">
                    <div class="card_count_wrapper">
                        <p class="title">Current Bid</p>
                        <div class="card_count">
                            <img src="~/assets/images/eth.png" alt="eth">
                            <p>0.25 ETH</p>
                        </div>
                    </div>
                    <div class="card_count_wrapper">
                        <p class="title">Ends in</p>
                        <div class="card_count">
                            <p>12h  43m  42s</p>
                        </div>
                    </div>
                </div>
            </label>
            <label for="s5" id="slide5" class="card-slider relative">
                <img class="card_image" src="~/assets/images/three.png" alt="one">
                <div class="card_caption_one">
                    <div class="caption_title">Abstr Gradient NFT</div>
                    <div class="caption_owner">
                        <img src="~/assets/images/owner.png" alt="owner">
                        <p>Arkhan17</p>
                    </div>
                </div>
                <div class="card_caption_two">
                    <div class="card_count_wrapper">
                        <p class="title">Current Bid</p>
                        <div class="card_count">
                            <img src="~/assets/images/eth.png" alt="eth">
                            <p>0.25 ETH</p>
                        </div>
                    </div>
                    <div class="card_count_wrapper">
                        <p class="title">Ends in</p>
                        <div class="card_count">
                            <p>12h  43m  42s</p>
                        </div>
                    </div>
                </div>
            </label>
        </section>
    </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>
    .card_caption_two {
        @apply absolute left-0 right-0 bottom-0 flex items-center justify-between px-[26px] py-[15px] m-[26px];
        background: rgba(255, 255, 255, 0.2);
        backdrop-filter: blur(25px);
        border-radius: 12px;
    }
    .card_count_wrapper {

    }
    .card_count_wrapper .title {
        @apply font-[500] text-[12px] leading-[16px] text-[#FFFFFF] mb-[8px]; 
    }
    .card_count {
        @apply flex items-center gap-[10px];
    }
    .card_count p {
        @apply font-[700] text-[16px] leading-[21px] text-[#FFFFFF]; 
    }
    .card_caption_one {
        @apply absolute top-[26px] left-[26px];
    }
    .caption_title {
        @apply font-[700] text-[28px] leading-[36px] tracking-[-0.05em] text-[#FFFFFF] mb-[10px]; 
    }
    .caption_owner {
        @apply flex items-center gap-[15px];
    }
    .caption_owner p{
        @apply font-[700] text-[20px] leading-[26px] text-[#FFFFFF];
    }
    .card_image {
        @apply w-full h-full;
    }
    [type=radio] {
        display: none;
    }

    #slider {
        @apply h-auto relative;
        perspective: 1000px;
        transform-style: preserve-3d;
    }

    #slider label {
        margin: auto;
        border-radius: 4px;
        position: absolute;
        left: 0; right: 0;
        cursor: pointer;
        transition: transform 0.4s ease;
        border-radius: 24px;
    }

    #s1:checked ~ #slide4, #s2:checked ~ #slide5,
    #s3:checked ~ #slide1, #s4:checked ~ #slide2,
    #s5:checked ~ #slide3 {
        box-shadow: 0 1px 4px 0 rgba(0,0,0,.37);
        transform: translate3d(-30%,0,-200px);
        margin-top: 40px;
    }

    #s1:checked ~ #slide5, #s2:checked ~ #slide1,
    #s3:checked ~ #slide2, #s4:checked ~ #slide3,
    #s5:checked ~ #slide4 {
        box-shadow: 0 6px 10px 0 rgba(0,0,0,.3), 0 2px 2px 0 rgba(0,0,0,.2);
        transform: translate3d(-15%,0,-100px);
        margin-top: 20px;
    }

    #s1:checked ~ #slide1, #s2:checked ~ #slide2,
    #s3:checked ~ #slide3, #s4:checked ~ #slide4,
    #s5:checked ~ #slide5 {
        box-shadow: 0 13px 25px 0 rgba(0,0,0,.3), 0 11px 7px 0 rgba(0,0,0,.19);
        transform: translate3d(0,0,0);
    }

    #s1:checked ~ #slide2, #s2:checked ~ #slide3,
    #s3:checked ~ #slide4, #s4:checked ~ #slide5,
    #s5:checked ~ #slide1 {
        box-shadow: 0 6px 10px 0 rgba(0,0,0,.3), 0 2px 2px 0 rgba(0,0,0,.2);
        transform: translate3d(15%,0,-100px);
        margin-top: 20px;
    }

    #s1:checked ~ #slide3, #s2:checked ~ #slide4,
    #s3:checked ~ #slide5, #s4:checked ~ #slide1,
    #s5:checked ~ #slide2 {
        box-shadow: 0 1px 4px 0 rgba(0,0,0,.37);
        transform: translate3d(30%,0,-200px);
        margin-top: 40px;
    }
    .card-slider {
        background: #fff;
        width: 378px;
        height: 440px;
    }
</style>