<template>
    <div style="min-height: 100vh;" class="search-act-container">
        <div class="banner-container">
            <swiper :modules="[SwiperNavigation, SwiperAutoplay]">

                <swiper-slide>

                    <div class="image">
                        <img src="../assets/images/banner1.avif" alt="">
                    </div>

                </swiper-slide>
                <!-- <div class="arrows">
                    <div class="arrow slider-banner-next">
                        <i class="fa-solid fa-chevron-left"></i>
                    </div>
                    <div class="arrow slider-banner-prev">
                        <i class="fa-solid fa-chevron-right"></i>
                    </div>
                </div> -->
            </swiper>
            <div class="search-container">
                <div class="search-input">
                    <div class="d-flex align-items-center w-100 gap-2">
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20" fill="none">
                            <path
                                d="M19.2577 18.0152L15.0838 13.8396C16.3353 12.2088 16.9195 10.163 16.7181 8.11728C16.5167 6.07154 15.5446 4.17901 13.9991 2.82361C12.4537 1.46821 10.4505 0.751427 8.39594 0.818668C6.3414 0.885908 4.38937 1.73214 2.93581 3.18569C1.48226 4.63924 0.63603 6.59128 0.56879 8.64581C0.50155 10.7003 1.21833 12.7035 2.57373 14.249C3.92914 15.7945 5.82166 16.7666 7.86741 16.968C9.91315 17.1694 11.9589 16.5852 13.5897 15.3337L17.7671 19.5119C17.8652 19.61 17.9816 19.6879 18.1098 19.741C18.238 19.794 18.3754 19.8214 18.5141 19.8214C18.6529 19.8214 18.7902 19.794 18.9184 19.741C19.0466 19.6879 19.1631 19.61 19.2612 19.5119C19.3593 19.4138 19.4371 19.2974 19.4902 19.1692C19.5433 19.041 19.5706 18.9036 19.5706 18.7649C19.5706 18.6261 19.5433 18.4888 19.4902 18.3606C19.4371 18.2324 19.3593 18.1159 19.2612 18.0178L19.2577 18.0152ZM2.69151 8.91783C2.69151 7.7358 3.04203 6.58032 3.69873 5.5975C4.35542 4.61468 5.28882 3.84866 6.38087 3.39632C7.47292 2.94398 8.67458 2.82563 9.83389 3.05623C10.9932 3.28683 12.0581 3.85603 12.8939 4.69185C13.7297 5.52767 14.2989 6.59257 14.5295 7.75188C14.7601 8.9112 14.6418 10.1129 14.1895 11.2049C13.7371 12.297 12.9711 13.2304 11.9883 13.8871C11.0055 14.5437 9.84998 14.8943 8.66795 14.8943C7.0834 14.8926 5.56422 14.2625 4.44377 13.142C3.32332 12.0216 2.69314 10.5024 2.69151 8.91783Z"
                                fill="#5E5E5E" />
                        </svg>
                        <input type="text" v-model="searchText" class="w-100" placeholder="Search Activities">
                        <!-- <span> Search Activities </span> -->
                    </div>
                    <v-menu activator="parent">
                        <div class="search-box">
                            <div class="main-act">
                                <div v-for="item in filterArr" class="act-box">
                                    <div class="image">
                                        <img src="../assets/images/act1.png" alt="">
                                    </div>
                                    <div class="text">
                                        <h5> {{ item.title }} </h5>
                                        <span> Dubai City , United Arab Emirates </span>
                                    </div>
                                </div>

                            </div>
                        </div>
                    </v-menu>
                </div>

            </div>
        </div>

        <div class="container top-search">
            <h1> Top Abu Dhabi Tours & Activities </h1>
            <div class="main">
                <div class="arrow slider-search-prev">

                    <svg xmlns="http://www.w3.org/2000/svg" width="31" height="31" viewBox="0 0 31 31" fill="none">
                        <g>
                            <path d="M17.893 9.63361L11.6592 15.8675L17.893 22.1014" stroke="black"
                                stroke-width="1.87016" stroke-linecap="round" stroke-linejoin="round" />
                        </g>
                    </svg>
                </div>
                <swiper :navigation="{
                nextEl: '.slider-search-next',
                prevEl: '.slider-search-prev',
            }" :autoplay="{
                delay: 4500,
                disableOnInteraction: false,
            }" :modules="[SwiperNavigation, SwiperAutoplay]" :breakpoints="{
                '300': {
                    slidesPerView: 2,
                    spaceBetween: 20,
                },
                '768': {
                    slidesPerView: 4,
                    spaceBetween: 40,
                },
                '1024': {
                    slidesPerView: 7,
                    spaceBetween: 30,
                },
            }">
                    <swiper-slide v-for="i in 13">
                        <div class="box">
                            <img src="../assets/images/act2.png" alt="">
                            <h6> Desert safari
                                Tours </h6>

                        </div>
                    </swiper-slide>
                </swiper>

                <div class="arrow slider-search-next">
                    <svg xmlns="http://www.w3.org/2000/svg" width="31" height="31" viewBox="0 0 31 31" fill="none">
                        <path d="M12.9078 22.1002L19.1416 15.8662L12.9078 9.63232" stroke="black" stroke-width="1.87016"
                            stroke-linecap="round" stroke-linejoin="round" />
                    </svg>
                </div>

            </div>
        </div>

        <div class="container things-text">
            <h5> Things To Do In Abu Dhabi </h5>
            <p>

                {{ check1 ? text1.substring(0, 355) : text1 }} ... <span @click="check1 = !check1"> {{ check1 ?
                    'Readmore' : 'Read less' }} </span>

            </p>
        </div>

        <div class="container filter-container">
            <div class="header w-100 d-flex align-items-center justify-content-between">
                <div class="d-flex align-items-center gap-3">
                    <div class="d-flex align-items-center gap-2">
                        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 28 28" fill="none">
                            <path
                                d="M14.002 2.62402C11.7522 2.62402 9.55296 3.29116 7.68235 4.54106C5.81174 5.79096 4.35378 7.56749 3.49283 9.646C2.63188 11.7245 2.40662 14.0116 2.84553 16.2182C3.28443 18.4247 4.3678 20.4515 5.95862 22.0424C7.54944 23.6332 9.57627 24.7165 11.7828 25.1555C13.9893 25.5944 16.2765 25.3691 18.355 24.5082C20.4335 23.6472 22.21 22.1892 23.4599 20.3186C24.7098 18.448 25.377 16.2488 25.377 13.999C25.3738 10.9832 24.1743 8.09174 22.0418 5.9592C19.9092 3.82666 17.0178 2.62721 14.002 2.62402ZM23.627 13.999C23.6279 15.2338 23.3902 16.4572 22.927 17.6018L18.0379 14.5951C17.83 14.4668 17.5975 14.3837 17.3554 14.3512L14.8595 14.0143C14.5155 13.9695 14.166 14.0271 13.8547 14.1801C13.5434 14.333 13.2842 14.5744 13.1095 14.874H12.1557L11.7401 14.0143C11.6252 13.775 11.457 13.565 11.2485 13.4007C11.0399 13.2363 10.7966 13.1219 10.537 13.0661L9.66196 12.8768L10.5173 11.374H12.3449C12.6407 11.3734 12.9315 11.2982 13.1904 11.1553L14.5302 10.4159C14.648 10.3503 14.758 10.2718 14.8584 10.1818L17.8016 7.51965C18.0967 7.25519 18.2929 6.89805 18.3577 6.50713C18.4225 6.11622 18.3521 5.71488 18.1582 5.36934L18.1188 5.29824C19.7658 6.07918 21.1575 7.31117 22.1325 8.85124C23.1074 10.3913 23.6256 12.1763 23.627 13.999ZM15.6765 4.52059L16.627 6.22246L13.6837 8.88465L12.3449 9.62402H10.5173C10.2096 9.62357 9.90733 9.70422 9.64081 9.85783C9.37428 10.0114 9.15296 10.2326 8.99915 10.499L8.0443 12.1648L6.93415 9.2073L8.13071 6.37777C9.18983 5.55942 10.4082 4.97132 11.7078 4.65113C13.0074 4.33094 14.3595 4.28573 15.6776 4.5184L15.6765 4.52059ZM4.37696 13.999C4.3755 12.5684 4.69467 11.1557 5.31102 9.86465L6.55133 13.1754C6.6547 13.4495 6.82522 13.6933 7.04728 13.8844C7.26933 14.0755 7.53581 14.2078 7.82227 14.2692L10.1662 14.7734L10.5829 15.6396C10.7275 15.9343 10.9516 16.1826 11.23 16.3565C11.5083 16.5305 11.8297 16.6231 12.1579 16.624H12.3198L11.529 18.3992C11.3897 18.7118 11.345 19.0583 11.4006 19.396C11.4562 19.7337 11.6096 20.0476 11.8418 20.299L11.8571 20.3143L14.002 22.5237L13.7898 23.6175C11.2761 23.559 8.88491 22.5204 7.12634 20.7234C5.36777 18.9264 4.38113 16.5133 4.37696 13.999ZM15.5966 23.4906L15.7202 22.8551C15.771 22.5851 15.7579 22.307 15.682 22.043C15.606 21.779 15.4693 21.5365 15.2827 21.3348C15.2774 21.33 15.2723 21.3249 15.2674 21.3195L13.127 19.1112L14.6254 15.749L17.1213 16.0859L22.122 19.1615C21.3975 20.2993 20.4424 21.2724 19.3184 22.0181C18.1944 22.7638 16.9266 23.2654 15.5966 23.4906Z"
                                fill="#FF733C" />
                        </svg>
                        <h4> 19 Things to do in Abu Dhabi </h4>
                    </div>
                    <div class="btns">
                        <button class="active"> View All Tours </button>
                        <button> Super Saver Tours </button>
                    </div>
                </div>

                <div class="filter">
                    <button>
                        <span class="">
                            Most Popular
                        </span>

                        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="5" viewBox="0 0 10 5" fill="none">
                            <path d="M4.83552 4.83594L-0.000843048 -0.000421524L9.67188 -0.000421524L4.83552 4.83594Z"
                                fill="black" />
                        </svg>

                        <v-menu activator="parent">
                            <div class="mostP-modal py-3 px-2" style="background-color: #fff;">
                                <div class="d-flex flex-column gap-4">
                                    <span> Most Popular </span>
                                    <span> Price Low To High </span>
                                    <span> Price High To Low </span>
                                    <span> Top Rated </span>
                                    <span> Recommended </span>
                                </div>
                            </div>
                        </v-menu>
                    </button>
                    <button>
                        <span class="">
                            Price Range
                        </span>

                        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="5" viewBox="0 0 10 5" fill="none">
                            <path d="M4.83552 4.83594L-0.000843048 -0.000421524L9.67188 -0.000421524L4.83552 4.83594Z"
                                fill="black" />
                        </svg>

                        <v-menu activator="parent">
                            <div class="price-range-modal">
                                <v-range-slider color="#fd7037" v-model="value" :min="minPrice" :max="maxPrice"
                                    step="50" strict></v-range-slider>
                                <div class="w-100 d-flex align-items-center justify-content-between">
                                    <span> {{ value[0] }} </span>
                                    <span> {{ value[1] }} </span>
                                </div>
                            </div>
                        </v-menu>
                    </button>
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
                                    <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 12 12"
                                        fill="none">
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

            <v-pagination v-model="page" :length="20" rounded="circle" class="my-4"></v-pagination>
        </div>
    </div>
</template>

<script setup>
let page = ref(1);
let searchText = ref('');

let minPrice = ref(0);
let maxPrice = ref(400);

let value = ref([20, 40]);



let text1 = ref('Known to the world a some of the best cities to live in, Abu Dhabi has worked hard over the past decade and created a niche for itself in the tourism industry away from the shadow of the mighty Dubai. Abu Dhabi city tours are now one of the most sought after tours in the UAE and the Middle East. The capital city of UAE with a population of roughly under jdklajsdka aksldjaksld askdjlka fsl;dk flkasdjflkas dflkasdhlf adlskfhlasdjfhals dfhlajsdhflasd flasdfl');
let check1 = ref(true);
let actArr = ref([
    {
        title: "3D Blacklight Minigolf Dubai",
        desc: "Dubai City , United Arab Emirates"
    },
    {
        title: "3D World Selfie Museum",
        desc: "Dubai City , United Arab Emirates"
    },
    {
        title: "6 Emirates In A Day Tour",
        desc: "Dubai City , United Arab Emirates"
    },
    {
        title: "Abu Dhabi City Tour",
        desc: "Dubai City , United Arab Emirates"
    },
    {
        title: "Abu Dhabi City Tour With Ferraraior Yas transfers",
        desc: "Dubai City , United Arab Emirates"
    },
    {
        title: "bb Blacklight Minigolf Dubai",
        desc: "Dubai City , United Arab Emirates"
    },
]);


let filterArr = computed(() => {
    return actArr.value.filter((ele) => {
        console.log(ele.title.toLowerCase().includes(searchText.value.toLowerCase()));
        return ele.title.toLowerCase().includes(searchText.value.toLowerCase());
    });
});

</script>

<style lang="scss" scoped></style>