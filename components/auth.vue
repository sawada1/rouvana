<template>

    <div class="modal" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="auth-container">

                    <div class=" login">
                        <div class="head">
                            <button @click="loginBtn1 = 1" :class="{ 'active': loginBtn1 == 1 }"> login now
                            </button>
                            <button @click="loginBtn1 = 2" :class="{ 'active': loginBtn1 == 2 }"> my booking
                            </button>
                        </div>

                        <div v-if="loginBtn1 == 1">
                            <p>
                                Sign in to unlock a world of rewards - accumulate Rayna Tours Loyalty points or snag
                                exclusive
                                discounts on your booked travel experiences!

                            </p>


                            <div class="social-auth">
                                <div class="box">
                                    <img src="../assets/images/devicon_google.svg" alt="">
                                    <span> Sign in with google </span>
                                </div>
                                <div class="box">
                                    <img src="../assets/images/logos_facebook.svg" alt="">
                                    <span> Sign in with facebook </span>
                                </div>
                            </div>

                            <div class="line">
                                <span> Or sign in with email </span>
                            </div>

                            <div class="inputs">
                                <div class="inputs-container">
                                    <div>
                                        <input type="email" placeholder="Email address">

                                    </div>
                                    <div>
                                        <input type="password" placeholder="Password">

                                    </div>

                                </div>
                                <div class="forget-remember d-flex align-items-center justify-content-between">
                                    <div class="d-flex align-items-center gap-2">
                                        <input id="rem1" type="checkbox">
                                        <label for="rem1">remember me</label>
                                    </div>
                                    <span class="forget"> Forgot Password? </span>
                                </div>

                                <button> LOG IN </button>
                            </div>

                            <div class="line">

                            </div>

                            <div class="d-flex foot align-items-center flex-column flex-xl-row flex-lg-row gap-2 justify-content-between w-100">
                                <span> No account yet? Sign up now ! </span>
                                <button> Sign Up </button>
                            </div>

                        </div>
                        <div v-if="loginBtn1 == 2">
                            <p>
                                View/ Print/Cancel Your Booking without Signing in
                            </p>

                            <div class="inputs">
                                <div class="inputs-container">
                                    <div>
                                        <input type="email" placeholder="Email address">

                                    </div>
                                    <div>
                                        <input type="number" placeholder="Booking Reference Number">

                                    </div>

                                </div>

                                <button> SUBMIT </button>
                            </div>

                        </div>


                        <button class="close" data-bs-dismiss="modal" aria-label="Close">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none">
                                <path
                                    d="M2.51172 24.001L0.124023 21.6133L9.67481 12.0625L0.124023 2.51172L2.51172 0.124023L12.0625 9.67481L21.6133 0.124023L24.001 2.51172L14.4502 12.0625L24.001 21.6133L21.6133 24.001L12.0625 14.4502L2.51172 24.001Z"
                                    fill="#F4F3F3" />
                            </svg>
                        </button>
                    </div>

                </div>

            </div>
        </div>
    </div>
</template>


<script setup>
let loginBtn1 = ref(1);
</script>