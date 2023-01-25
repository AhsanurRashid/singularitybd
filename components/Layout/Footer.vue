<template>
  <footer>
    <section id="footer_section">
        <div class="footer_container">
            <div class="footer_row">
                <div class="footer_col_one">
                    <div class="logo">
                        <h1>NFters</h1>
                    </div>
                    <div class="description">
                        <p>The world’s first and largest digital marketplace for crypto collectibles and non-fungible tokens (NFTs). Buy, sell, and discover exclusive digital items.</p>
                    </div>
                    <div class="socila_medias">
                        <img src="~/assets/images/facebook.png" alt="facebook">
                        <img src="~/assets/images/twitter.png" alt="twitter">
                        <img src="~/assets/images/linkedin.png" alt="linkedin">
                    </div>
                </div>
                <div class="footer_col_two">
                    <div>
                        <div class="footer_title">
                            <p>Market Place</p>
                        </div>
                        <ul class="list">
                            <li>All NFTs</li>
                            <li>New</li>
                            <li>Art</li>
                            <li>Sports</li>
                            <li>Utility</li>
                            <li>Music</li>
                            <li>Domain Name</li>
                        </ul>
                    </div>
                    <div>
                        <div class="footer_title">
                            <p>My Account</p>
                        </div>
                        <ul class="list">
                            <li>Profile</li>
                            <li>Favorite</li>
                            <li>My Collections</li>
                            <li>Settings</li>
                        </ul>
                    </div>
                </div>
                <div class="footer_col_three">
                    <div class="footer_title">
                        <p>Stay in the loop</p>
                    </div>
                    <div class="description">
                        <p>Join our mailing list to stay in the loop with our newest feature releases, NFT drops, and tips and tricks for navigating NFTs.</p>
                    </div>
                    <div class="subscibe_now">
                        <input type="text" placeholder="Enter your email address..">
                        <div class="subscibe_now_btn">Subscibe Now</div>
                    </div>
                </div>
            </div>
            <div class="copyright">
                Copyright © 2022 Avi Yansah
            </div>
        </div>
    </section>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
    footer {
        @apply bg-white;
    }
    #footer_section {
        @apply pt-[79px];
    }
    .footer_container {
        @apply container mx-auto;
    }
    .footer_row {
        @apply grid grid-cols-3 gap-[100px] pb-[79px] border-b border-[#F4F4F4]; 
    }
    .footer_col_one .logo{
        @apply font-[700] text-[24px] leading-[29px] text-[#000000] uppercase mb-[27px];
    }
    .footer_col_one .description{
        @apply font-[400] text-[14px] leading-[160%] text-[#565656] mb-[32px];
    }
    .footer_col_one .socila_medias{
        @apply flex items-center gap-[16px] cursor-pointer;
    }
    .footer_title {
        @apply font-[700] text-[18px] leading-[23px] capitalize text-main mb-[24px];
    }
    .footer_col_three .description{
        @apply font-[400] text-[14px] leading-[160%] text-[#565656] mb-[24px];
    }
    .subscibe_now {
        @apply relative w-full;
    }
    .subscibe_now input{
        @apply w-full outline-none focus:outline-none py-[22.4px] pl-[26px] pr-[150px] border-2 border-[#F1F1F1]  focus:border-primary rounded-[45.595px] text-[12.1587px] leading-[16px] font-[400] text-main placeholder:text-[#959595];
    }
    .subscibe_now_btn {
        @apply absolute top-[9px] right-[9px] shadow font-[400] text-[12.1587px] leading-[16px] tracking-[0.065em] text-[#FFFFFF] px-[30px] py-[15px] bg-primary rounded-[45.595px] cursor-pointer;
    }
    .footer_col_two {
        @apply grid grid-cols-2 gap-[100px];
    }
    .list {
        @apply mb-[24px];
    }
    .list li{
        @apply font-[500] text-[14px] leading-[200%] text-[#3D3D3D] cursor-pointer transition-all ease-in-out duration-75 delay-75 hover:text-primary no-underline hover:underline;
    }
    .copyright {
        @apply font-[400] text-[14px] leading-[160%] text-[#A4A4A4] text-center py-[24px];
    }
</style>