<template>
  <section id="amazingnft_section">
    <div class="amazingnft_container">
        <div class="amazingnft_row">
            <div class="amazingnft_col flex items-center">
                <h1>The amazing NFT art of the world here</h1>
            </div>
            <div class="amazingnft_col">
                <div class="flex items-start gap-[15px]">
                    <img src="~/assets/images/card.png" alt="card">
                    <div>
                        <h3>Fast Transaction</h3>
                        <p class="w-[60%]">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam etiam viverra tellus imperdiet.</p>
                    </div>
                </div>
            </div>
            <div class="amazingnft_col">
                <div class="flex items-start gap-[15px]">
                    <img src="~/assets/images/graph.png" alt="graph">
                    <div>
                        <h3>Growth Transaction</h3>
                        <p class="w-[74%]">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam etiam viverra tellus</p>
                    </div>
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
    #amazingnft_section {
        background: rgba(217, 224, 236, 0.2);
        backdrop-filter: blur(25px);
    }
    .amazingnft_container {
        @apply container mx-auto py-[122px]; 
    }
    .amazingnft_row {
        @apply grid grid-cols-3;
    }   
    .amazingnft_col {

    }
    .amazingnft_col h1{
        @apply w-[80%] font-[700] text-[28px] leading-[34px] text-main uppercase;
    }
    .amazingnft_col h3{
        @apply font-[700] text-[20px] leading-[26px] text-main mb-[12px] mt-[6px];
    }
    .amazingnft_col p{
        @apply font-light text-[14px] leading-[160%] text-[#696969];
    }
</style>