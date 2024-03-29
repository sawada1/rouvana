<template>

    <div style="min-height:100vh">

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
            <div class="search-container">
                <div class="search-input">
                    <div class="d-flex align-items-center gap-2">
                        <i class="fa-solid fa-location-dot"></i>
                        <span> select location </span>
                    </div>
                    <v-menu activator="parent">
                        <div class="search-box">
                            <div class="row">
                                <div v-for="i in 5" class="col-6 col-xl-3 col-lg-3">
                                    <div class="box">
                                        <img src="../assets/images/abu-dhabi.png" alt="">
                                        <span> Abu Dhabi </span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </v-menu>
                </div>

            </div>
        </div>

        <div class="container">
            <div class="main-boxes-home">
                <div class="header">
                    <div>
                        <h3> Most Popular Experiences in Dubai </h3>
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
                        <h3> Top Experiences in Abu Dhabi </h3>
                        <p> Discover the best attractions and activities that the UAE's capital city has to offer.
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

    </div>

</template>


<script setup>

</script>