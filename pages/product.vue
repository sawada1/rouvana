<template>
  <div class="main-product-page" style="min-height: 100vh">
    <div class="container slider">
      <swiper :navigation="true" :modules="[SwiperNavigation, SwiperAutoplay]">
        <swiper-slide v-for="i in 4">
          <div class="image">
            <img src="../assets/images/act2.png" alt="" />
          </div>
        </swiper-slide>
      </swiper>
      <div class="title">
        <div class="d-flex align-items-center gap-2">
          <h5>Qasr Al Watan Abu Dhabi</h5>
          <div class="d-flex align-items-center gap-2">
            <v-rating v-model="rating" size="x-small" length="5" color="#fd7037" density="comfortable"
              readonly></v-rating>
            <span class="rate"> 68 Reviews </span>
          </div>
        </div>
      </div>
      <div class="details">
        <span class="save"> Save up to 5.00 Per Person </span>
        <span class="earn"> Earn 1500 R Points </span>
        <div class="d-flex price align-items-center gap-3">
          <span> From AED 65.00 </span>
          <h4>AED 60.00</h4>
        </div>
        <button>BOOK NOW</button>
      </div>
    </div>
    <div class="container line-container">
      <div class="item">
        <span> operating hours </span>

        <div class="tooltipp">
          <span> everyday: 10am - to 6:00pm</span>
        </div>
      </div>
      <div class="item">
        <span> operating hours </span>
        <div class="tooltipp">
          <span> everyday: 10am - to 6:00pm</span>
        </div>
      </div>
      <div class="item">
        <span> operating hours </span>
        <div class="tooltipp">
          <span> everyday: 10am - to 6:00pm</span>
        </div>
      </div>
      <div class="item">
        <span> operating hours </span>

      </div>
      <div class="item">
        <span> operating hours </span>
      </div>
      <div class="item">
        <span> operating hours </span>
      </div>
      <div class="item">
        <span> operating hours </span>
      </div>
    </div>

    <div class=" container offers-price-container">
      <div class="title">
        <h4> Qasr Al Watan Abu Dhabi Price & Offers </h4>
      </div>


      <div class="main-table">

        <div class="table-container">

          <table class="main-table">
            <thead>
              <tr>
                <td class="head-table first"> Tour Option </td>
                <td class="head-table bord">
                  transfer option
                  <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 15 15" fill="none">
                    <path
                      d="M7.5 1.40625C6.29477 1.40625 5.11661 1.76364 4.1145 2.43323C3.11238 3.10282 2.33133 4.05454 1.87011 5.16802C1.40889 6.28151 1.28821 7.50676 1.52334 8.68883C1.75847 9.8709 2.33884 10.9567 3.19107 11.8089C4.0433 12.6612 5.1291 13.2415 6.31117 13.4767C7.49324 13.7118 8.71849 13.5911 9.83198 13.1299C10.9455 12.6687 11.8972 11.8876 12.5668 10.8855C13.2364 9.88339 13.5938 8.70523 13.5938 7.5C13.592 5.88436 12.9495 4.33538 11.807 3.19295C10.6646 2.05052 9.11564 1.40796 7.5 1.40625ZM7.5 12.6562C6.48019 12.6562 5.48328 12.3538 4.63534 11.7873C3.7874 11.2207 3.12651 10.4154 2.73625 9.47321C2.34598 8.53103 2.24387 7.49428 2.44283 6.49407C2.64178 5.49385 3.13287 4.5751 3.85398 3.85398C4.5751 3.13287 5.49385 2.64178 6.49407 2.44283C7.49428 2.24387 8.53103 2.34598 9.47321 2.73625C10.4154 3.12651 11.2207 3.7874 11.7873 4.63534C12.3538 5.48328 12.6563 6.48019 12.6563 7.5C12.6547 8.86705 12.111 10.1777 11.1443 11.1443C10.1777 12.111 8.86705 12.6547 7.5 12.6562ZM7.03125 7.96875V4.6875C7.03125 4.56318 7.08064 4.44395 7.16855 4.35604C7.25645 4.26814 7.37568 4.21875 7.5 4.21875C7.62432 4.21875 7.74355 4.26814 7.83146 4.35604C7.91937 4.44395 7.96875 4.56318 7.96875 4.6875V7.96875C7.96875 8.09307 7.91937 8.2123 7.83146 8.30021C7.74355 8.38811 7.62432 8.4375 7.5 8.4375C7.37568 8.4375 7.25645 8.38811 7.16855 8.30021C7.08064 8.2123 7.03125 8.09307 7.03125 7.96875ZM8.20313 10.0781C8.20313 10.2172 8.16189 10.3531 8.08463 10.4688C8.00737 10.5844 7.89756 10.6745 7.76908 10.7277C7.6406 10.7809 7.49922 10.7949 7.36283 10.7677C7.22644 10.7406 7.10115 10.6736 7.00282 10.5753C6.90448 10.477 6.83752 10.3517 6.81039 10.2153C6.78326 10.0789 6.79718 9.93753 6.8504 9.80905C6.90362 9.68057 6.99374 9.57076 7.10937 9.4935C7.225 9.41624 7.36094 9.375 7.5 9.375C7.68648 9.375 7.86533 9.44908 7.99719 9.58094C8.12905 9.7128 8.20313 9.89164 8.20313 10.0781Z"
                      fill="#E33629" />
                  </svg>
                  <div class="tooltipp">
                    <div class="mainn d-flex flex-column gap-1">
                      <p>
                        we have multiple transfer options for this
                        tour so pleasw select any of the transfer
                        option from the list

                      </p>

                      <p>
                        <span> Without Transfers </span>- No transfers will be
                        Provided

                      </p>
                      <p>
                        <span> Sharing Transfers </span>
                        - During your tour you’ll
                        be sharing the vehicle with some more
                        people

                      </p>
                      <p>
                        <span> Private Transfers </span>
                        - During your tour you’ll
                        be provided private vehicle and you won’t
                        be sharing this vehicle with anyone
                        <span> Hourly</span>
                        - Private tours on hourly basis

                      </p>

                    </div>
                  </div>
                </td>
                <td class="head-table "> tour date </td>
                <td class="head-table "> Adult </td>
                <td class="head-table "> Child </td>
                <td class="head-table "> infant </td>
                <td class="head-table bord">
                  total amount
                  <svg class="total" xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 15 15"
                    fill="none">
                    <path
                      d="M7.5 1.40625C6.29477 1.40625 5.11661 1.76364 4.1145 2.43323C3.11238 3.10282 2.33133 4.05454 1.87011 5.16802C1.40889 6.28151 1.28821 7.50676 1.52334 8.68883C1.75847 9.8709 2.33884 10.9567 3.19107 11.8089C4.0433 12.6612 5.1291 13.2415 6.31117 13.4767C7.49324 13.7118 8.71849 13.5911 9.83198 13.1299C10.9455 12.6687 11.8972 11.8876 12.5668 10.8855C13.2364 9.88339 13.5938 8.70523 13.5938 7.5C13.592 5.88436 12.9495 4.33538 11.807 3.19295C10.6646 2.05052 9.11564 1.40796 7.5 1.40625ZM7.5 12.6562C6.48019 12.6562 5.48328 12.3538 4.63534 11.7873C3.7874 11.2207 3.12651 10.4154 2.73625 9.47321C2.34598 8.53103 2.24387 7.49428 2.44283 6.49407C2.64178 5.49385 3.13287 4.5751 3.85398 3.85398C4.5751 3.13287 5.49385 2.64178 6.49407 2.44283C7.49428 2.24387 8.53103 2.34598 9.47321 2.73625C10.4154 3.12651 11.2207 3.7874 11.7873 4.63534C12.3538 5.48328 12.6563 6.48019 12.6563 7.5C12.6547 8.86705 12.111 10.1777 11.1443 11.1443C10.1777 12.111 8.86705 12.6547 7.5 12.6562ZM7.03125 7.96875V4.6875C7.03125 4.56318 7.08064 4.44395 7.16855 4.35604C7.25645 4.26814 7.37568 4.21875 7.5 4.21875C7.62432 4.21875 7.74355 4.26814 7.83146 4.35604C7.91937 4.44395 7.96875 4.56318 7.96875 4.6875V7.96875C7.96875 8.09307 7.91937 8.2123 7.83146 8.30021C7.74355 8.38811 7.62432 8.4375 7.5 8.4375C7.37568 8.4375 7.25645 8.38811 7.16855 8.30021C7.08064 8.2123 7.03125 8.09307 7.03125 7.96875ZM8.20313 10.0781C8.20313 10.2172 8.16189 10.3531 8.08463 10.4688C8.00737 10.5844 7.89756 10.6745 7.76908 10.7277C7.6406 10.7809 7.49922 10.7949 7.36283 10.7677C7.22644 10.7406 7.10115 10.6736 7.00282 10.5753C6.90448 10.477 6.83752 10.3517 6.81039 10.2153C6.78326 10.0789 6.79718 9.93753 6.8504 9.80905C6.90362 9.68057 6.99374 9.57076 7.10937 9.4935C7.225 9.41624 7.36094 9.375 7.5 9.375C7.68648 9.375 7.86533 9.44908 7.99719 9.58094C8.12905 9.7128 8.20313 9.89164 8.20313 10.0781Z"
                      fill="#E33629" />
                  </svg>
                  <div class="tooltipp sec">
                    <span> We offer you A rate tag bespoke to your
                      Pocket and specifications. Book online &
                      make your payment using credit card or via
                      bank transfer </span>
                  </div>
                </td>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>
                  <div class="input">
                    <div class="d-flex flex-column ">
                      <div class="d-flex align-items-center gap-3">
                        <input id="check-inp-1" type="checkbox">
                        <label for="check-inp-1"> Qasr Al-Watan - Palace and Garden (Admission Only)</label>
                        <v-dialog transition="dialog-top-transition" width="auto">
                          <template v-slot:activator="{ props: activatorProps }">
                            <button class="info" v-bind="activatorProps"> More Info </button>
                          </template>
                          <template v-slot:default="{ isActive }">
                            <div class="more-info-container">
                              <div class="main">
                                <div class="head">
                                  <h3> Qasr Al Watan Abu Dhabi </h3>
                                </div>
                                <div class="body">
                                  <div class="item ">
                                    <div class="d-flex align-items-cente gap-2">
                                      <div class="icon">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="3" viewBox="0 0 10 3"
                                          fill="none">
                                          <path d="M0.666992 1.5H9.61144" stroke="white" stroke-width="2.55556" />
                                        </svg>
                                      </div>
                                      <div class="d-flex flex-column mt-1  align-items-cente">
                                        <h6> Voucher Confirmation </h6>
                                        <div class="main-item">
                                          <svg xmlns="http://www.w3.org/2000/svg" width="31" height="31"
                                            viewBox="0 0 31 31" fill="none">
                                            <path
                                              d="M24.5827 16.5083L13.5481 5.47376C13.3836 5.30796 13.1878 5.17651 12.9721 5.08705C12.7563 4.99758 12.525 4.9519 12.2914 4.95265H1.99242C1.75667 4.95265 1.53058 5.0463 1.36388 5.213C1.19718 5.3797 1.10352 5.60579 1.10352 5.84154V16.1405C1.10278 16.3741 1.14846 16.6055 1.23793 16.8212C1.32739 17.0369 1.45884 17.2327 1.62464 17.3972L12.6592 28.4318C12.8243 28.5969 13.0203 28.7279 13.236 28.8173C13.4517 28.9066 13.6829 28.9526 13.9164 28.9526C14.1499 28.9526 14.3811 28.9066 14.5969 28.8173C14.8126 28.7279 15.0086 28.5969 15.1737 28.4318L24.5827 19.0228C24.7478 18.8577 24.8788 18.6617 24.9681 18.446C25.0575 18.2303 25.1035 17.9991 25.1035 17.7656C25.1035 17.5321 25.0575 17.3009 24.9681 17.0851C24.8788 16.8694 24.7478 16.6734 24.5827 16.5083ZM13.9159 27.1751L2.88132 16.1405V6.73044H12.2914L23.326 17.765L13.9159 27.1751ZM8.21471 10.7305C8.21471 10.9942 8.13651 11.252 7.99 11.4713C7.84349 11.6905 7.63525 11.8614 7.39161 11.9623C7.14798 12.0633 6.87989 12.0897 6.62124 12.0382C6.3626 11.9868 6.12502 11.8598 5.93855 11.6733C5.75207 11.4868 5.62508 11.2493 5.57364 10.9906C5.52219 10.732 5.54859 10.4639 5.64951 10.2202C5.75043 9.9766 5.92133 9.76836 6.1406 9.62185C6.35986 9.47534 6.61765 9.39714 6.88136 9.39714C7.23499 9.39714 7.57413 9.53762 7.82418 9.78767C8.07424 10.0377 8.21471 10.3769 8.21471 10.7305Z"
                                              fill="#FD7037" />
                                          </svg>
                                          <div class="d-flex flex-column gap-1">
                                            <h6> Mobile Voucher </h6>
                                            <p> Use Your phone or Print Your voucher </p>
                                          </div>
                                        </div>

                                      </div>
                                    </div>
                                  </div>
                                  <div class="item ">
                                    <div class="d-flex align-items-cente gap-2">
                                      <div class="icon">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="3" viewBox="0 0 10 3"
                                          fill="none">
                                          <path d="M0.666992 1.5H9.61144" stroke="white" stroke-width="2.55556" />
                                        </svg>
                                      </div>
                                      <div class="d-flex flex-column mt-1  align-items-cente">
                                        <h6> Booking Confirmation</h6>
                                        <div class="main-item">
                                          <svg xmlns="http://www.w3.org/2000/svg" width="21" height="28"
                                            viewBox="0 0 21 28" fill="none">
                                            <path
                                              d="M20.8535 13.2553C20.8191 13.1096 20.7492 12.9747 20.6501 12.8625C20.551 12.7504 20.4257 12.6644 20.2854 12.6123L13.7405 10.1572L15.406 1.82633C15.4437 1.63276 15.4174 1.43219 15.3311 1.25486C15.2448 1.07753 15.1032 0.933082 14.9276 0.843303C14.7521 0.753524 14.552 0.723289 14.3578 0.75716C14.1635 0.791031 13.9855 0.887171 13.8507 1.03107L1.12657 14.664C1.02323 14.7729 0.94847 14.9057 0.908972 15.0506C0.869475 15.1954 0.866471 15.3478 0.900228 15.4941C0.933985 15.6403 1.00345 15.776 1.10242 15.8889C1.20139 16.0017 1.32679 16.0883 1.4674 16.1409L8.01463 18.596L6.35368 26.9178C6.31597 27.1114 6.34223 27.3119 6.42852 27.4893C6.5148 27.6666 6.65642 27.811 6.832 27.9008C7.00758 27.9906 7.2076 28.0208 7.40187 27.987C7.59615 27.9531 7.77413 27.857 7.90897 27.7131L20.6331 14.0801C20.7345 13.9712 20.8077 13.839 20.8461 13.6952C20.8846 13.5514 20.8871 13.4003 20.8535 13.2553ZM8.76331 24.1424L9.95278 18.1916C9.99535 17.9805 9.96162 17.7612 9.85759 17.5727C9.75356 17.3842 9.586 17.2388 9.38474 17.1623L3.38169 14.9072L12.9952 4.60745L11.8069 10.5582C11.7643 10.7693 11.798 10.9886 11.9021 11.1771C12.0061 11.3656 12.1737 11.511 12.3749 11.5875L18.3734 13.837L8.76331 24.1424Z"
                                              fill="#FD7037" />
                                          </svg>
                                          <div class="d-flex flex-column gap-1">
                                            <h6>Instant Confirmation </h6>
                                            <p> Instant Tour Confirmation will be Provided </p>
                                          </div>
                                        </div>

                                      </div>
                                    </div>
                                  </div>
                                  <div class="item ">
                                    <div class="d-flex align-items-cente gap-2">
                                      <div class="icon">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="3" viewBox="0 0 10 3"
                                          fill="none">
                                          <path d="M0.666992 1.5H9.61144" stroke="white" stroke-width="2.55556" />
                                        </svg>
                                      </div>
                                      <div class="d-flex flex-column mt-1 w-100 align-items-cente">
                                        <h6> Timings & Duration</h6>
                                        <div class="main-item w-100">
                                          <div class="main-container">
                                            <div
                                              class="header d-flex align-items-center  w-100 justify-content-between">
                                              <h6>Transfer Type </h6>
                                              <h6>Pickup Timings</h6>
                                              <h6>Duration Approx</h6>
                                            </div>
                                            <div v-for="i in 3"
                                              class="d-flex align-items-center  w-100 justify-content-between">
                                              <span> Sharing Transfers </span>
                                              <span class="main-text"> Morning Pick up 10:00 AM | Drop Off 02:30 PM
                                                Afternoon Pick up
                                                05:00 PM | Drop Off 09:30 PM</span>
                                              <span> 04:30 hours </span>
                                            </div>

                                          </div>
                                        </div>

                                      </div>
                                    </div>
                                  </div>
                                  <div class="item ">
                                    <div class="d-flex align-items-cente gap-2">
                                      <div class="icon">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="3" viewBox="0 0 10 3"
                                          fill="none">
                                          <path d="M0.666992 1.5H9.61144" stroke="white" stroke-width="2.55556" />
                                        </svg>
                                      </div>
                                      <div class="d-flex flex-column mt-1  align-items-cente">
                                        <h6> Booking Policy </h6>
                                        <div class="main-item">

                                          <div class="d-flex flex-column gap-3">
                                            <h6> Cancellation Policy </h6>
                                            <div v-for="i in 6" class="d-flex align-items-center mb-2 gap-3">
                                              <svg xmlns="http://www.w3.org/2000/svg" width="6" height="6"
                                                viewBox="0 0 6 6" fill="none">
                                                <circle cx="3" cy="3" r="3" fill="#FD7037" />
                                              </svg>
                                              <h6> All Cancellations made 72 hours prior to the Tour departure time NO
                                                charges will be applicable </h6>

                                            </div>

                                          </div>

                                        </div>

                                      </div>
                                    </div>
                                  </div>
                                </div>
                              </div>
                              <!-- <v-btn text="Close" @click="isActive.value = false"></v-btn> -->
                              <svg class="close" @click="isActive.value = false" xmlns="http://www.w3.org/2000/svg"
                                width="56" height="51" viewBox="0 0 56 51" fill="none">
                                <ellipse cx="29.9554" cy="25.5" rx="25.9554" ry="25.5" fill="#FD7037" />
                                <path
                                  d="M21.1745 36.7451L19 34.5706L27.698 25.8725L19 17.1745L21.1745 15L29.8725 23.698L38.5706 15L40.7451 17.1745L32.047 25.8725L40.7451 34.5706L38.5706 36.7451L29.8725 28.047L21.1745 36.7451Z"
                                  fill="#F4F3F3" />
                              </svg>

                            </div>
                          </template>
                        </v-dialog>
                        <!-- <button class="info"> More Info </button> -->
                      </div>

                      <span> Select Time Slot </span>
                      <span> Not Refundable </span>

                    </div>
                  </div>
                </td>
                <td>
                  <!-- <div class="select">
                    <select>
                      <option value=""> Without Transfers</option>
                      <option value=""> Without Transfers</option>
                      <option value=""> Without Transfers</option>
                      <option value=""> Without Transfers</option>
                    </select>
                   
                  </div> -->
                  <button class="select">
                    <span>
                      Without Transfers

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span> Without Transfers </span>
                        <span>Sharing Transfers </span>
                        <span> Private Transfers </span>
                      </div>
                    </v-menu>
                  </button>
                </td>
                <td>
                  <input type="date">
                </td>
                <td>
                  <button class="select">
                    <span>
                      Without Transfers

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span> Without Transfers </span>
                        <span>Sharing Transfers </span>
                        <span> Private Transfers </span>
                      </div>
                    </v-menu>
                  </button>
                </td>
                <td>
                  <button class="select">
                    <span>
                      0

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span v-for="i, index in 20"> {{ index }} </span>
                      </div>
                    </v-menu>
                  </button>
                </td>
                <td> <button class="select">
                    <span>
                      0

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span v-for="i, index in 20"> {{ index }} </span>

                      </div>
                    </v-menu>
                  </button></td>
                <td>
                  <div class="price">
                    <span class="disc"> AED 65.00 </span>
                    <h5> AED 60.00 </h5>
                    <v-dialog transition="dialog-top-transition" width="auto">
                      <template v-slot:activator="{ props: activatorProps }">
                        <button class="save" style="font-size: 11px;" v-bind="activatorProps"> Save 500 </button>
                      </template>
                      <template v-slot:default="{ isActive }">
                        <div class="more-info-container">
                          <div class="main">
                            <div class="head">
                              <h3> Your Price Quote Details </h3>
                            </div>
                            <div class="body">


                              <div class="item ">
                                <div class="d-flex align-items-cente gap-2">
                                  <div class="icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="10" height="3" viewBox="0 0 10 3"
                                      fill="none">
                                      <path d="M0.666992 1.5H9.61144" stroke="white" stroke-width="2.55556" />
                                    </svg>
                                  </div>
                                  <div class="d-flex flex-column mt-1 w-100 align-items-cente">
                                    <h6> Your Price Quote Details</h6>
                                    <div class="main-item w-100">
                                      <div class="table-container">
                                        <div class="headerr">
                                          Your Guarantee lowest price for this option is based on the following:
                                        </div>
                                        <table class="table table-borderless">
                                          <thead>
                                            <tr>
                                              <th> Tour Option </th>
                                              <th> Transfer Option </th>
                                              <th> Adult </th>
                                              <th> PriceChild </th>
                                              <th> PriceTotal </th>
                                            </tr>
                                          </thead>
                                          <tbody>
                                            <tr>
                                              <td> Qasr Al Watan - Palace and Garden (Admission Only) </td>
                                              <td> Without Transfers</td>
                                              <td> AED 60.00 X 1 </td>
                                              <td> AED 30.00 X 0 </td>
                                              <td> AED 60.00 </td>
                                            </tr>
                                          </tbody>
                                        </table>

                                      </div>
                                    </div>

                                  </div>
                                </div>
                              </div>

                              <div class="price-table">
                                <h4> Your total cost: AED 60.00 </h4>
                              </div>

                            </div>
                          </div>
                          <!-- <v-btn text="Close" @click="isActive.value = false"></v-btn> -->
                          <svg class="close" @click="isActive.value = false" xmlns="http://www.w3.org/2000/svg"
                            width="56" height="51" viewBox="0 0 56 51" fill="none">
                            <ellipse cx="29.9554" cy="25.5" rx="25.9554" ry="25.5" fill="#FD7037" />
                            <path
                              d="M21.1745 36.7451L19 34.5706L27.698 25.8725L19 17.1745L21.1745 15L29.8725 23.698L38.5706 15L40.7451 17.1745L32.047 25.8725L40.7451 34.5706L38.5706 36.7451L29.8725 28.047L21.1745 36.7451Z"
                              fill="#F4F3F3" />
                          </svg>

                        </div>
                      </template>
                    </v-dialog>
                    <span class="earn"> Earn 1500 R Points </span>
                  </div>
                </td>
              </tr>
              <tr>
                <td>
                  <div class="input">
                    <div class="d-flex flex-column ">
                      <div class="d-flex align-items-center gap-3">
                        <input id="check-inp-1" type="checkbox">
                        <label for="check-inp-1"> Qasr Al-Watan - Palace and Garden (Admission Only)</label>
                        <button class="info"> More Info </button>
                      </div>

                      <span> Select Time Slot </span>
                      <span> Not Refundable </span>

                    </div>
                  </div>
                </td>
                <td>
                  <!-- <div class="select">
                    <select>
                      <option value=""> Without Transfers</option>
                      <option value=""> Without Transfers</option>
                      <option value=""> Without Transfers</option>
                      <option value=""> Without Transfers</option>
                    </select>
                   
                  </div> -->
                  <button class="select">
                    <span>
                      Without Transfers

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span> Without Transfers </span>
                        <span>Sharing Transfers </span>
                        <span> Private Transfers </span>
                      </div>
                    </v-menu>
                  </button>
                </td>
                <td>
                  <input type="date">
                </td>
                <td>
                  <button class="select">
                    <span>
                      Without Transfers

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span> Without Transfers </span>
                        <span>Sharing Transfers </span>
                        <span> Private Transfers </span>
                      </div>
                    </v-menu>
                  </button>
                </td>
                <td>
                  <button class="select">
                    <span>
                      0

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span v-for="i, index in 20"> {{ index }} </span>
                      </div>
                    </v-menu>
                  </button>
                </td>
                <td> <button class="select">
                    <span>
                      0

                    </span>
                    <svg xmlns="http://www.w3.org/2000/svg" width="8" height="7" viewBox="0 0 8 7" fill="none">
                      <path d="M1 0.5L4 5.5L7.5 0.5" stroke="#423D3D" />
                    </svg>
                    <v-menu activator="parent">
                      <div class="select-drop">
                        <span v-for="i, index in 20"> {{ index }} </span>

                      </div>
                    </v-menu>
                  </button></td>
                <td>
                  <div class="price">
                    <span class="disc"> AED 65.00 </span>
                    <h5> AED 60.00 </h5>
                    <span class="save"> Save 500 </span>
                    <span class="earn"> Earn 1500 R Points </span>
                  </div>
                </td>
              </tr>

            </tbody>
          </table>
        </div>
      </div>


    </div>

    <div class="container text-details-container">
      <div>
        <h4> Qasr Al Watan Abu Dhabi Overview </h4>
        <p> Escape from Abu Dhabi’s usual sights and find your way to the extraordinary Qasr Al Watan or the Palace of
          the Nation! A striking segment of the capital city’s Presidential Palace complex, Qasr Al Watan is where the
          significant government buildings are located. Besides the meeting place of the country’s supreme
          constitutional authority, it also serves as a venue to host the global leaders during their UAE visit. As it’s
          now opened to the public, come trace the footprints of royals while gaining a better understanding of the
          Emirati culture, heritage and architectural opulence.

          Experience one of the finest in the Royal Arabian architecture as you step inside the facility and find
          yourself under the country’s largest central dome. Watch videos displaying the intriguing facets of the palace
          architecture and further work your way across its diverse sections enriched by intricate, attention to detail
          artistry. Admire the massive chandeliers with over 300,000 crystal pieces, discover the Room of Gifts with the
          choicest items on display, check out the House of Knowledge, and marvel at the extravagance of the
          Presidential Banquet area, among others.

          There are many attractions that allow for immersive experiences; try producing fascinating calligraphy on
          interactive screens and spectacle an evening light and sound show which not only steps you back in time but
          also journeys you through present and into the future. Featuring a vast array of authentic publications on the
          region’s culture, history, archaeology, and constitution, Qasr Al Watan library deserves a special mention
          too. You’ll also get to explore the lush landscape surrounding the palace. Take a walk under the elegantly
          tranquil archways and get the best views of palace from its lawn. </p>
      </div>
    </div>
    <div class="container text-details-container">
      <div>
        <h4> Qasr Al Watan Abu Dhabi Highlights </h4>
        <div class="lines">
          <div v-for="i in 5" class="line">
            <svg xmlns="http://www.w3.org/2000/svg" width="6" height="6" viewBox="0 0 6 6" fill="none">
              <circle cx="3" cy="3" r="3" fill="#FD7037" />
            </svg>
            <span> Walk in the footsteps of dignitaries and world leaders as you step into Qasr Al Watan inside the Abu
              Dhabi Presidential Complex. </span>
          </div>
        </div>
      </div>
    </div>
    <div class="container text-details-container">
      <div>
        <h4> Qasr Al Watan Abu Dhabi Itinerary </h4>
        <div class="lines">
          <div v-for="i in 5" class="line">
            <svg xmlns="http://www.w3.org/2000/svg" width="6" height="6" viewBox="0 0 6 6" fill="none">
              <circle cx="3" cy="3" r="3" fill="#FD7037" />
            </svg>
            <span> Walk in the footsteps of dignitaries and world leaders as you step into Qasr Al Watan inside the Abu
              Dhabi Presidential Complex. </span>
          </div>
        </div>
      </div>
    </div>
    <div class="container text-details-container">
      <div>
        <h4> Qasr Al Watan Abu Dhabi Important Information </h4>
        <div class="lines">
          <div v-for="i in 5" class="line">
            <svg xmlns="http://www.w3.org/2000/svg" width="6" height="6" viewBox="0 0 6 6" fill="none">
              <circle cx="3" cy="3" r="3" fill="#FD7037" />
            </svg>
            <span> Walk in the footsteps of dignitaries and world leaders as you step into Qasr Al Watan inside the Abu
              Dhabi Presidential Complex. </span>
          </div>
        </div>
      </div>
    </div>
    <div class="container text-details-container">
      <div>
        <h4> Qasr Al Watan Abu Dhabi Location </h4>
        <div class="location">
          <span> Location Name </span>
          <img src="../assets/images/map.png" alt="">
        </div>
      </div>
    </div>
    <div class="container text-details-container last">
      <div>
        <h4> Qasr Al Watan Abu Dhabi Reviews </h4>
        <div class="main-review">
          <div class="header">
            <div class="rate d-flex flex-column align-items-center">
              <span> 5.5 / 5.5 </span>
              <svg xmlns="http://www.w3.org/2000/svg" width="142" height="26" viewBox="0 0 142 26" fill="none">
                <path
                  d="M12.9785 0L16.4114 8.01082L25.3218 8.70416L18.533 14.3485L20.6071 22.7878L12.9785 18.2653L5.34993 22.7878L7.42402 14.3485L0.635213 8.70416L9.54564 8.01082L12.9785 0Z"
                  fill="#FD7037" />
                <path
                  d="M41.9892 0L45.4221 8.01082L54.3325 8.70416L47.5437 14.3485L49.6178 22.7878L41.9892 18.2653L34.3607 22.7878L36.4348 14.3485L29.646 8.70416L38.5564 8.01082L41.9892 0Z"
                  fill="#FD7037" />
                <path
                  d="M71 0L74.4328 8.01082L83.3433 8.70416L76.5545 14.3485L78.6285 22.7878L71 18.2653L63.3714 22.7878L65.4455 14.3485L58.6567 8.70416L67.5671 8.01082L71 0Z"
                  fill="#FD7037" />
                <path
                  d="M100.011 0L103.444 8.01082L112.354 8.70416L105.565 14.3485L107.639 22.7878L100.011 18.2653L92.3822 22.7878L94.4562 14.3485L87.6674 8.70416L96.5779 8.01082L100.011 0Z"
                  fill="#FD7037" />
                <path
                  d="M129.021 0L132.454 8.01082L141.365 8.70416L134.576 14.3485L136.65 22.7878L129.021 18.2653L121.393 22.7878L123.467 14.3485L116.678 8.70416L125.589 8.01082L129.021 0Z"
                  fill="#FD7037" />
              </svg>
            </div>

            <div class="stars-container">
              <div v-for="i in 4" class="item">
                <div class="d-flex align-items-center gap-2">
                  <span> 5 star</span>
                  <svg xmlns="http://www.w3.org/2000/svg" width="63" height="11" viewBox="0 0 63 11" fill="none">
                    <path
                      d="M5.71054 0L7.22099 3.52476L11.1416 3.82983L8.15451 6.31332L9.06711 10.0266L5.71054 8.03674L2.35397 10.0266L3.26657 6.31332L0.279494 3.82983L4.20008 3.52476L5.71054 0Z"
                      fill="#FD7037" />
                    <path
                      d="M18.4752 0L19.9856 3.52476L23.9062 3.82983L20.9192 6.31332L21.8318 10.0266L18.4752 8.03674L15.1186 10.0266L16.0312 6.31332L13.0441 3.82983L16.9647 3.52476L18.4752 0Z"
                      fill="#FD7037" />
                    <path
                      d="M31.2398 0L32.7503 3.52476L36.6709 3.82983L33.6838 6.31332L34.5964 10.0266L31.2398 8.03674L27.8833 10.0266L28.7959 6.31332L25.8088 3.82983L29.7294 3.52476L31.2398 0Z"
                      fill="#FD7037" />
                    <path
                      d="M44.0045 0L45.5149 3.52476L49.4355 3.82983L46.4485 6.31332L47.3611 10.0266L44.0045 8.03674L40.6479 10.0266L41.5605 6.31332L38.5734 3.82983L42.494 3.52476L44.0045 0Z"
                      fill="#FD7037" />
                    <path
                      d="M56.7691 0L58.2796 3.52476L62.2002 3.82983L59.2131 6.31332L60.1257 10.0266L56.7691 8.03674L53.4126 10.0266L54.3252 6.31332L51.3381 3.82983L55.2587 3.52476L56.7691 0Z"
                      fill="#FD7037" />
                  </svg>
                </div>
                <div class="progress-container">
                  <div class="progresss">
                    <div class="back"></div>
                  </div>
                  <span> 68 </span>
                </div>
              </div>
            </div>
          </div>

          <div class="rates-container">

            <div v-for="i in 3" class="item">
              <div class="image">
                <img src="../assets/images/kk.jpg">
                <span> Sameer M </span>
                <span> August 2023 </span>
              </div>
              <div class="divider"></div>
              <div class="text">
                <h6> Superlative Architecture </h6>
                <p> Qasr Al Watan is a stunning edifice constructed with white granite and attractive artworks that
                  features complex yet
                  beautiful inlay designs all over are captivating </p>
              </div>
              <div class="theRate">
                <span> 5.0/5.0 </span>
                <svg xmlns="http://www.w3.org/2000/svg" width="54" height="10" viewBox="0 0 54 10" fill="none">
                  <path
                    d="M5.68287 0.137695L6.95895 3.11554L10.2712 3.37327L7.74762 5.47141L8.51862 8.60855L5.68287 6.92742L2.84711 8.60855L3.61811 5.47141L1.09452 3.37327L4.40678 3.11554L5.68287 0.137695Z"
                    fill="#FD7037" />
                  <path
                    d="M16.468 0.137695L17.7441 3.11554L21.0564 3.37327L18.5328 5.47141L19.3038 8.60855L16.468 6.92742L13.6323 8.60855L14.4033 5.47141L11.8797 3.37327L15.1919 3.11554L16.468 0.137695Z"
                    fill="#FD7037" />
                  <path
                    d="M27.2512 0.137695L28.5273 3.11554L31.8396 3.37327L29.316 5.47141L30.087 8.60855L27.2512 6.92742L24.4155 8.60855L25.1865 5.47141L22.6629 3.37327L25.9751 3.11554L27.2512 0.137695Z"
                    fill="#FD7037" />
                  <path
                    d="M38.0354 0.137695L39.3115 3.11554L42.6237 3.37327L40.1002 5.47141L40.8712 8.60855L38.0354 6.92742L35.1997 8.60855L35.9707 5.47141L33.4471 3.37327L36.7593 3.11554L38.0354 0.137695Z"
                    fill="#FD7037" />
                  <path
                    d="M48.8196 0.137695L50.0957 3.11554L53.4079 3.37327L50.8843 5.47141L51.6553 8.60855L48.8196 6.92742L45.9838 8.60855L46.7548 5.47141L44.2312 3.37327L47.5435 3.11554L48.8196 0.137695Z"
                    fill="#FD7037" />
                </svg>
                <div class="stat"> Excellent </div>
              </div>
            </div>

            <div class="w-100 d-flex justify-content-center align-items-center">

              <button class="more"> show more </button>

            </div>

          </div>
        </div>
      </div>



    </div>

  </div>
</template>

<script setup>
let rating = ref(5);
</script>

<style lang="scss" scoped></style>
