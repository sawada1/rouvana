<template>
    <div style="min-height: 100vh;">
        <div>
            <div class="banner-container">
                <swiper :navigation="{
                    nextEl: '.slider-banner-next',
                    prevEl: '.slider-banner-prev',
                }" :autoplay="{
                    delay: 4500,
                    disableOnInteraction: false,
                }" :modules="[SwiperNavigation, SwiperAutoplay]">

                    <swiper-slide v-for="i in 6">

                        <div class="image">
                            <img src="../assets/images/banner1.avif" alt="">
                        </div>

                    </swiper-slide>
                    <div class="arrows">
                        <div class="arrow slider-banner-next">
                            <i class="fa-solid fa-chevron-left"></i>
                        </div>
                        <div class="arrow slider-banner-prev">
                            <i class="fa-solid fa-chevron-right"></i>
                        </div>
                    </div>
                </swiper>
                <div class="d-flex align-items-center justify-content-center gap-5">
                <div class="search-container  holidays">
                    <div class="search-input">
                        <div class="d-flex align-items-center gap-2">
                            <i class="fa-solid fa-location-dot"></i>
                            <span> Select Country </span>
                        </div>
                     <v-menu activator="parent">
                                <div class="search-box">
                                    <div class="">
                                        <div class="d-flex flex-column gap-2">
                                            <div v-for="i in 5" class="box hotels">
                                                <div class="arrow">
                                                  <svg xmlns="http://www.w3.org/2000/svg" width="12" height="14" viewBox="0 0 12 14" fill="none">
  <path d="M5.6 0C2.48792 0 0 2.33242 0 5.25C0 6.25898 0.320833 7.03828 0.877917 7.82852L5.01083 13.7074C5.13625 13.8852 5.35208 14 5.6 14C5.84792 14 6.06667 13.8824 6.18917 13.7074L10.3221 7.82852C10.8792 7.03828 11.2 6.25898 11.2 5.25C11.2 2.33242 8.71208 0 5.6 0ZM5.6 8.16484C3.88208 8.16484 2.48792 6.85781 2.48792 5.24453C2.48792 3.63125 3.88208 2.32422 5.6 2.32422C7.31792 2.32422 8.71208 3.63125 8.71208 5.24453C8.71208 6.85781 7.31792 8.16484 5.6 8.16484Z" fill="#423D3D"/>
</svg>
                                                    <div class="d-flex flex-column gap-1">
                                                        <span class="city"> Dublin </span>
                                                        <p class="m-0"> Ohio United States of America </p>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </v-menu>
                    </div>

                </div>
                <div class="search-container  holidays">
                    <div class="search-input">
                        <div class="d-flex align-items-center gap-2">
                            <i class="fa-solid fa-location-dot"></i>
                            <span> select location </span>
                        </div>
                <v-menu activator="parent">
                        <div class="search-box">
                            <div class="main-act">
                                <div v-for="item in 3" class="act-box">
                                    <div class="image">
                                        <img src="../assets/images/act1.png" alt="">
                                    </div>
                                    <div class="text">
                                        <h5> sasas </h5>
                                        <span> Dubai City , United Arab Emirates </span>
                                    </div>
                                </div>

                            </div>
                        </div>
                    </v-menu>
                    </div>

                </div>
                
                </div>
            </div>

            <div class="container top-cities">
                <div class="d-flex w-100 align-items-center justify-content-between mb-3">
                    <div class="text">
                        <h3> Holiday Destinations </h3>
                        <p>
                           Explore the most popular and trending places to travel around the world
                        </p>
                    </div>
                    <div class="arrows">
                        <div class="arrow slider-top-next">
                            <i class="fa-solid fa-chevron-left"></i>
                        </div>
                        <div class="arrow slider-top-prev">
                            <i class="fa-solid fa-chevron-right"></i>
                        </div>
                    </div>
                </div>

                <div class="row">
                <div v-for="i in 8" class="col-12 col-xl-3 mb-4 col-lg-3 col-md-6">
                 <div  class="box holiday">
                            <img src="../assets/images/abu-dhabi.png" alt="">
                            <h4> Abu Dhabi </h4>
                        </div>
                </div>
                </div>
                <!-- <swiper :navigation="{
                    nextEl: '.slider-top-next',
                    prevEl: '.slider-top-prev',
                }" :autoplay="{
                    delay: 4500,
                    disableOnInteraction: false,
                }" :modules="[SwiperNavigation, SwiperAutoplay]" :breakpoints="{
                    '300': {
                        slidesPerView: 2,
                        spaceBetween: 20,
                    },
                    '768': {
                        slidesPerView: 3,
                        spaceBetween: 40,
                    },
                    '1024': {
                        slidesPerView: 4,
                        spaceBetween: 50,
                    },
                }">
                    <swiper-slide v-for="i in 8">
                        <div class="box">
                            <img src="../assets/images/abu-dhabi.png" alt="">
                            <h4> Abu Dhabi </h4>
                        </div>
                    </swiper-slide>
                </swiper> -->

            </div>

            <div class="container">
                <div class="main-boxes-home">
                    <div class="header">
                        <div>
                            <h3> Trending Dubai Holidays (Without Flights) </h3>
                            <p> Culture, nature, thrills, and record-breaking experiences—Dubai is the place to seek out
                                everything you imagine and beyond. Find it all here! </p>
                        </div>
                        <div class="arrows">
                            <div class="arrow slider-top-next">
                                <i class="fa-solid fa-chevron-left"></i>
                            </div>
                            <div class="arrow slider-top-prev">
                                <i class="fa-solid fa-chevron-right"></i>
                            </div>
                        </div>
                    </div>
                    <swiper :navigation="{
                    nextEl: '.slider-top-next',
                    prevEl: '.slider-top-prev',
                }" :autoplay="{
                    delay: 4500,
                    disableOnInteraction: false,
                }" :modules="[SwiperNavigation, SwiperAutoplay]" :breakpoints="{
                    '300': {
                        slidesPerView: 2,
                        spaceBetween: 20,
                    },
                    '768': {
                        slidesPerView: 3,
                        spaceBetween: 40,
                    },
                    '1024': {
                        slidesPerView: 4,
                        spaceBetween: 20,
                    },
                }">
                        <swiper-slide v-for="i in 4">
                            <div class="box-card">
                                <div class="image">
                                    <img src="../assets/images/hotel1.png" alt="">
                                </div>
                                <div class="main">
                                    <h4> Paramotor Adventure Tour </h4>
                                    <div class="foot">
                                        <!-- <div class="earn">
                                            <span> Earn 1500 R Points </span>
                                            <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12"
                                                viewBox="0 0 12 12" fill="none">
                                                <path
                                                    d="M5.80476 1.5144C4.94766 1.5144 4.10981 1.76856 3.39716 2.24474C2.68451 2.72092 2.12906 3.39773 1.80107 4.18959C1.47307 4.98144 1.38725 5.85278 1.55446 6.69341C1.72167 7.53403 2.13441 8.3062 2.74046 8.91226C3.34652 9.51832 4.11869 9.93105 4.95932 10.0983C5.79995 10.2655 6.67129 10.1797 7.46314 9.85166C8.255 9.52366 8.93181 8.96822 9.40798 8.25557C9.88416 7.54292 10.1383 6.70507 10.1383 5.84797C10.1371 4.69901 9.68015 3.59745 8.86771 2.78502C8.05527 1.97258 6.95372 1.51562 5.80476 1.5144ZM5.80476 9.51483C5.07952 9.51483 4.37057 9.29977 3.76756 8.89685C3.16455 8.49393 2.69455 7.92125 2.41702 7.25122C2.13948 6.58118 2.06687 5.8439 2.20835 5.1326C2.34984 4.4213 2.69907 3.76793 3.21189 3.25511C3.72471 2.74229 4.37809 2.39305 5.08939 2.25156C5.80069 2.11008 6.53797 2.18269 7.20801 2.46023C7.87804 2.73777 8.45072 3.20776 8.85364 3.81077C9.25656 4.41378 9.47162 5.12273 9.47162 5.84797C9.47052 6.82014 9.08383 7.75218 8.3964 8.43961C7.70897 9.12704 6.77693 9.51373 5.80476 9.51483ZM5.47141 6.18132V3.84786C5.47141 3.75945 5.50653 3.67466 5.56904 3.61215C5.63156 3.54963 5.71635 3.51451 5.80476 3.51451C5.89317 3.51451 5.97796 3.54963 6.04047 3.61215C6.10299 3.67466 6.13811 3.75945 6.13811 3.84786V6.18132C6.13811 6.26973 6.10299 6.35452 6.04047 6.41703C5.97796 6.47955 5.89317 6.51467 5.80476 6.51467C5.71635 6.51467 5.63156 6.47955 5.56904 6.41703C5.50653 6.35452 5.47141 6.26973 5.47141 6.18132ZM6.30478 7.6814C6.30478 7.7803 6.27546 7.87697 6.22051 7.9592C6.16557 8.04143 6.08748 8.10552 5.99611 8.14336C5.90474 8.18121 5.8042 8.19111 5.70721 8.17182C5.61021 8.15252 5.52112 8.1049 5.45119 8.03497C5.38126 7.96504 5.33363 7.87595 5.31434 7.77895C5.29505 7.68195 5.30495 7.58142 5.34279 7.49005C5.38064 7.39868 5.44473 7.32059 5.52696 7.26564C5.60919 7.2107 5.70586 7.18137 5.80476 7.18137C5.93737 7.18137 6.06456 7.23405 6.15833 7.32783C6.2521 7.4216 6.30478 7.54878 6.30478 7.6814Z"
                                                    fill="#E33629" />
                                            </svg>
                                        </div> -->
                                        <div class="main-foot">
                                            <div class="rate">
                                                <span class="word"> 20 Reviews </span>
                                                <div class="d-flex align-items-center gap-2">
                                                    <svg v-for="i in 5" xmlns="http://www.w3.org/2000/svg" width="11"
                                                        height="10" viewBox="0 0 11 10" fill="none">
                                                        <path
                                                            d="M5.62054 0.587646L6.8741 4.1242H10.9307L7.64884 6.30991L8.9024 9.84645L5.62054 7.66075L2.33868 9.84645L3.59224 6.30991L0.310382 4.1242H4.36698L5.62054 0.587646Z"
                                                            fill="#FD7037" />
                                                    </svg>
                                                </div>
                                            </div>
                                            <div class="price">
                                                <span> AED 950.00 </span>
                                                <h6> AED 749.00 </h6>
                                            </div>

                                        </div>
                                    </div>

                                </div>
                            </div>
                        </swiper-slide>
                    </swiper>
                </div>
            </div>
            <div class="container">
                <div class="main-boxes-home">
                    <div class="header">
                        <div>
                            <h3> Eid Getaways </h3>
                            <p> Immerse yourself in the rich culture of Georgia, Armenia, Kazakhstan & Azerbaijan! Book your escape now.
                            </p>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-12 col-xl-3 col-lg-3 col-md-6 mb-5" v-for="i in 8">
                            <div class="box-card">
                                <div class="image">
                                    <img src="../assets/images/hotel1.png" alt="">
                                </div>
                                <div class="main w-100 h-100">
                                    <h4> Paramotor Adventure Tour </h4>
                                    <div class="foot">
                                        <div class="earn">
                                            <span> Earn 1500 R Points </span>
                                            <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12"
                                                viewBox="0 0 12 12" fill="none">
                                                <path
                                                    d="M5.80476 1.5144C4.94766 1.5144 4.10981 1.76856 3.39716 2.24474C2.68451 2.72092 2.12906 3.39773 1.80107 4.18959C1.47307 4.98144 1.38725 5.85278 1.55446 6.69341C1.72167 7.53403 2.13441 8.3062 2.74046 8.91226C3.34652 9.51832 4.11869 9.93105 4.95932 10.0983C5.79995 10.2655 6.67129 10.1797 7.46314 9.85166C8.255 9.52366 8.93181 8.96822 9.40798 8.25557C9.88416 7.54292 10.1383 6.70507 10.1383 5.84797C10.1371 4.69901 9.68015 3.59745 8.86771 2.78502C8.05527 1.97258 6.95372 1.51562 5.80476 1.5144ZM5.80476 9.51483C5.07952 9.51483 4.37057 9.29977 3.76756 8.89685C3.16455 8.49393 2.69455 7.92125 2.41702 7.25122C2.13948 6.58118 2.06687 5.8439 2.20835 5.1326C2.34984 4.4213 2.69907 3.76793 3.21189 3.25511C3.72471 2.74229 4.37809 2.39305 5.08939 2.25156C5.80069 2.11008 6.53797 2.18269 7.20801 2.46023C7.87804 2.73777 8.45072 3.20776 8.85364 3.81077C9.25656 4.41378 9.47162 5.12273 9.47162 5.84797C9.47052 6.82014 9.08383 7.75218 8.3964 8.43961C7.70897 9.12704 6.77693 9.51373 5.80476 9.51483ZM5.47141 6.18132V3.84786C5.47141 3.75945 5.50653 3.67466 5.56904 3.61215C5.63156 3.54963 5.71635 3.51451 5.80476 3.51451C5.89317 3.51451 5.97796 3.54963 6.04047 3.61215C6.10299 3.67466 6.13811 3.75945 6.13811 3.84786V6.18132C6.13811 6.26973 6.10299 6.35452 6.04047 6.41703C5.97796 6.47955 5.89317 6.51467 5.80476 6.51467C5.71635 6.51467 5.63156 6.47955 5.56904 6.41703C5.50653 6.35452 5.47141 6.26973 5.47141 6.18132ZM6.30478 7.6814C6.30478 7.7803 6.27546 7.87697 6.22051 7.9592C6.16557 8.04143 6.08748 8.10552 5.99611 8.14336C5.90474 8.18121 5.8042 8.19111 5.70721 8.17182C5.61021 8.15252 5.52112 8.1049 5.45119 8.03497C5.38126 7.96504 5.33363 7.87595 5.31434 7.77895C5.29505 7.68195 5.30495 7.58142 5.34279 7.49005C5.38064 7.39868 5.44473 7.32059 5.52696 7.26564C5.60919 7.2107 5.70586 7.18137 5.80476 7.18137C5.93737 7.18137 6.06456 7.23405 6.15833 7.32783C6.2521 7.4216 6.30478 7.54878 6.30478 7.6814Z"
                                                    fill="#E33629" />
                                            </svg>
                                        </div>
                                        <div class="main-foot">
                                            <div class="rate">
                                                <span class="word"> 20 Reviews </span>
                                                <div class="d-flex align-items-center gap-2">
                                                    <svg v-for="i in 5" xmlns="http://www.w3.org/2000/svg" width="11"
                                                        height="10" viewBox="0 0 11 10" fill="none">
                                                        <path
                                                            d="M5.62054 0.587646L6.8741 4.1242H10.9307L7.64884 6.30991L8.9024 9.84645L5.62054 7.66075L2.33868 9.84645L3.59224 6.30991L0.310382 4.1242H4.36698L5.62054 0.587646Z"
                                                            fill="#FD7037" />
                                                    </svg>
                                                </div>
                                            </div>
                                            <div class="price">
                                                <span> AED 950.00 </span>
                                                <h6> AED 749.00 </h6>
                                            </div>

                                        </div>
                                    </div>

                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="container">
                <div class="main-boxes-home">
                    <div class="header">
                        <div>
                            <h3> International Tour Packages </h3>
                            <div class="d-flex align-items-cente mt-2 gap-3">
                             <plane />
                            <p> Immerse yourself in the rich culture of Georgia, Armenia, Kazakhstan & Azerbaijan! Book your escape now.
                            </p>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-12 col-xl-3 col-lg-3 col-md-6 mb-5" v-for="i in 8">
                            <div class="box-card">
                                <div class="image">
                                    <img src="../assets/images/hotel1.png" alt="">
                                </div>
                                <div class="main w-100 h-100">
                                    <h4> Paramotor Adventure Tour </h4>
                                    <div class="foot">
                                        <div class="earn">
                                            <span> Earn 1500 R Points </span>
                                            <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12"
                                                viewBox="0 0 12 12" fill="none">
                                                <path
                                                    d="M5.80476 1.5144C4.94766 1.5144 4.10981 1.76856 3.39716 2.24474C2.68451 2.72092 2.12906 3.39773 1.80107 4.18959C1.47307 4.98144 1.38725 5.85278 1.55446 6.69341C1.72167 7.53403 2.13441 8.3062 2.74046 8.91226C3.34652 9.51832 4.11869 9.93105 4.95932 10.0983C5.79995 10.2655 6.67129 10.1797 7.46314 9.85166C8.255 9.52366 8.93181 8.96822 9.40798 8.25557C9.88416 7.54292 10.1383 6.70507 10.1383 5.84797C10.1371 4.69901 9.68015 3.59745 8.86771 2.78502C8.05527 1.97258 6.95372 1.51562 5.80476 1.5144ZM5.80476 9.51483C5.07952 9.51483 4.37057 9.29977 3.76756 8.89685C3.16455 8.49393 2.69455 7.92125 2.41702 7.25122C2.13948 6.58118 2.06687 5.8439 2.20835 5.1326C2.34984 4.4213 2.69907 3.76793 3.21189 3.25511C3.72471 2.74229 4.37809 2.39305 5.08939 2.25156C5.80069 2.11008 6.53797 2.18269 7.20801 2.46023C7.87804 2.73777 8.45072 3.20776 8.85364 3.81077C9.25656 4.41378 9.47162 5.12273 9.47162 5.84797C9.47052 6.82014 9.08383 7.75218 8.3964 8.43961C7.70897 9.12704 6.77693 9.51373 5.80476 9.51483ZM5.47141 6.18132V3.84786C5.47141 3.75945 5.50653 3.67466 5.56904 3.61215C5.63156 3.54963 5.71635 3.51451 5.80476 3.51451C5.89317 3.51451 5.97796 3.54963 6.04047 3.61215C6.10299 3.67466 6.13811 3.75945 6.13811 3.84786V6.18132C6.13811 6.26973 6.10299 6.35452 6.04047 6.41703C5.97796 6.47955 5.89317 6.51467 5.80476 6.51467C5.71635 6.51467 5.63156 6.47955 5.56904 6.41703C5.50653 6.35452 5.47141 6.26973 5.47141 6.18132ZM6.30478 7.6814C6.30478 7.7803 6.27546 7.87697 6.22051 7.9592C6.16557 8.04143 6.08748 8.10552 5.99611 8.14336C5.90474 8.18121 5.8042 8.19111 5.70721 8.17182C5.61021 8.15252 5.52112 8.1049 5.45119 8.03497C5.38126 7.96504 5.33363 7.87595 5.31434 7.77895C5.29505 7.68195 5.30495 7.58142 5.34279 7.49005C5.38064 7.39868 5.44473 7.32059 5.52696 7.26564C5.60919 7.2107 5.70586 7.18137 5.80476 7.18137C5.93737 7.18137 6.06456 7.23405 6.15833 7.32783C6.2521 7.4216 6.30478 7.54878 6.30478 7.6814Z"
                                                    fill="#E33629" />
                                            </svg>
                                        </div>
                                        <div class="main-foot">
                                            <div class="rate">
                                                <span class="word"> 20 Reviews </span>
                                                <div class="d-flex align-items-center gap-2">
                                                    <svg v-for="i in 5" xmlns="http://www.w3.org/2000/svg" width="11"
                                                        height="10" viewBox="0 0 11 10" fill="none">
                                                        <path
                                                            d="M5.62054 0.587646L6.8741 4.1242H10.9307L7.64884 6.30991L8.9024 9.84645L5.62054 7.66075L2.33868 9.84645L3.59224 6.30991L0.310382 4.1242H4.36698L5.62054 0.587646Z"
                                                            fill="#FD7037" />
                                                    </svg>
                                                </div>
                                            </div>
                                            <div class="price">
                                                <span> AED 950.00 </span>
                                                <h6> AED 749.00 </h6>
                                            </div>

                                        </div>
                                    </div>

                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
         
        </div>
    </div>
</template>

<script setup>
let cateBox = ref(1);
</script>

<style lang="scss" scoped></style>