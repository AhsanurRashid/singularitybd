<template>
  <header>
    <section id="header_section">
        <div class="header_container">
            <div class="header_row">
                <div class="header_col_one">
                    <div class="logo_and_menu">
                        <div class="logo">
                            <h1>NFters</h1>
                        </div>
                        <div class="menus">
                            <ul>
                                <li>Marketplace</li>
                                <li>Resource</li>
                                <li>About</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="header_col_two">
                    <div class="search_and_buttons">
                        <div class="search">
                            <input type="text" placeholder="Search">
                            <img class="search_btn" src="~/assets/images/search.png" alt="search">
                        </div>
                        <div class="upload">
                            Upload
                        </div>
                        <div class="Wallet">
                            Connect Wallet
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>
    header{
        
    }
    #header_section {
        @apply bg-white py-[31px] shadow-md;
        box-shadow: rgba(0, 0, 0, 0.16) 0px 0px 4px;
    }
    .header_container {
        @apply container mx-auto;
    }
    .header_row {
        @apply grid grid-cols-2;
    }
    .header_col_one {
        @apply flex items-center justify-start;
    }
    .logo_and_menu {
        @apply flex items-center;
    }
    .logo {
        @apply h-[47px] pr-[31px] border-r border-[#F4F4F4] flex items-center mr-[31px];
    }
    .logo h1 {
        font-family: 'MyTitleFont', Fallback, sans-serif;
        @apply font-bold text-primary text-[24px] leading-[29px] uppercase;
    }
    .menus {

    }
    .menus ul {
        @apply flex items-center gap-[47px];
    }
    .menus ul li {
        @apply font-medium text-[16px] leading-[21px] tracking-[0.04em] text-main cursor-pointer transition-all ease-in-out duration-75 delay-75 hover:text-primary;
    }

    .header_col_two {
        @apply flex items-center justify-end;
    }
    .search_and_buttons {
        @apply flex items-center gap-[20px];
    }
    .search {
        @apply relative;
    }
    .search input {
        @apply w-[300px] outline-none focus:outline-none border-2 border-gray-300 focus:border-primary py-[13px] pl-[30px] pr-[60px] rounded-[100px] text-main placeholder:text-[#C0C0C0] text-[16px] leading-[21px] tracking-[0.04em] placeholder:text-[16px] placeholder:leading-[21px] placeholder:tracking-[0.04em] placeholder:font-[500];
    }
    .search_btn {
        @apply absolute top-[14px] right-[20px] cursor-pointer;
    }
    .upload {
        @apply font-[700] text-[14px] leading-[100%] tracking-[0.04em] text-[#FFFFFF] bg-primary py-[18px] px-[40px] rounded-[60px] cursor-pointer;
    }
    .Wallet {
        @apply font-[700] text-[13px] leading-[100%] tracking-[0.04em] text-primary py-[18px] px-[22px] rounded-[60px] border-2 border-primary cursor-pointer;
    }   
</style>