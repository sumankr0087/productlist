<template>
    <div class="flex flex-col w-full">
        <div class="w-full max-w-screen-lg mx-auto">
            <div class='mt-8'>
                <div class="mb-2 text-[22px] text-[#333333] leading-8 font-normal font-serif">All European brands</div>
                <p class="text-[#333333] text-sm font-extralight">Shop independent brands from around the world at
                    wholesale prices.</p>
            </div>
        </div>
        <div class="mt-6">
            <div class='pt-2'>
                <div class="grid grid-cols-4 gap-x-2 gap-y-4">
                    <div v-for="product in productdata" :key="product.id"
                        class="w-full h-full flex flex-col relative bg-white">
                        <div class="w-full h-full relative bg-white border border-gray-300 flex flex-col">
                            <img class="border" alt="Mad Beauty in All European brands" :src="product.image">
                            <div class="w-8 h-8 absolute top-[42%] flex items-center flex-row justify-center">
                                <svg class="w-4 previous opacity-0" focusable="false" viewBox="0 0 24 24" aria-hidden="true"
                                    role="presentation" direction="left" fill="none" stroke-width="2">
                                    <path
                                        d="M6.60693 0.857147L17.1429 11.3931C17.2228 11.4728 17.2861 11.5674 17.3293 11.6715C17.3725 11.7756 17.3948 11.8873 17.3948 12C17.3948 12.1127 17.3725 12.2244 17.3293 12.3285C17.2861 12.4327 17.2228 12.5272 17.1429 12.6069L6.60693 23.1429"
                                        stroke="currentColor" stroke-linecap="round" stroke-linejoin="round">
                                    </path>
                                </svg>
                            </div>
                            <div class="w-8 h-8 absolute top-[42%] right-0 flex items-center flex-row justify-center">
                                <svg class="w-4 next opacity-0" focusable="false" viewBox="0 0 24 24" aria-hidden="true"
                                    role="presentation" direction="right" fill="none" stroke-width="2">
                                    <path
                                        d="M6.60693 0.857147L17.1429 11.3931C17.2228 11.4728 17.2861 11.5674 17.3293 11.6715C17.3725 11.7756 17.3948 11.8873 17.3948 12C17.3948 12.1127 17.3725 12.2244 17.3293 12.3285C17.2861 12.4327 17.2228 12.5272 17.1429 12.6069L6.60693 23.1429"
                                        stroke="currentColor" stroke-linecap="round" stroke-linejoin="round">
                                    </path>
                                </svg>
                            </div>
                            <div class="m-auto">
                                <div class="flex flex-row">
                                    <div class="w-2 h-1 relative mt-2 mb-3">
                                        <div
                                            class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-1 h-1 rounded-full bg-[#333333]">
                                        </div>
                                    </div>
                                    <div class="w-2 h-1 relative mt-2 mb-3">
                                        <div
                                            class=" absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-1 h-1 rounded-full bg-[#F7F7F7]">
                                        </div>
                                    </div>
                                    <div class="w-2 h-1 relative mt-2 mb-3">
                                        <div
                                            class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-1 h-1 rounded-full bg-[#F7F7F7]">
                                        </div>
                                    </div>
                                    <div class=" w-2 h-1 relative mt-2 mb-3">
                                        <div
                                            class=" absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-1 h-1 rounded-full bg-[#F7F7F7]">
                                        </div>
                                    </div>
                                    <div class=" w-2 h-1 relative mt-2 mb-3">
                                        <div
                                            class=" absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-1 h-1 rounded-full bg-[#F7F7F7]">
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div>
                                <div class="flex items-center flex-row justify-center pb-1">
                                    <div class="flex flex-start flex-col">
                                        <p class="font-medium text-sm text-[#333333]">
                                            {{ product.title }}
                                        </p>
                                    </div>
                                </div>
                                <div class=" pb-2 flex items-center flex-row justify-center">
                                    <div class="flex items-center flex-row">
                                        <svg class="text-[#333333] h-3 pr-1" focusable="false" viewBox="0 0 24 24"
                                            aria-hidden="true" role="presentation" color="#333333" fill="none"
                                            font-size="12px">
                                            <path
                                                d="M12.8436 1.87024L15.5573 7.37138C15.625 7.50794 15.7247 7.62606 15.8481 7.71563C15.9714 7.8052 16.1145 7.86355 16.2653 7.88566L22.3373 8.77024C22.5104 8.79635 22.6727 8.87028 22.806 8.9837C22.9392 9.09711 23.0382 9.2455 23.0917 9.41214C23.1451 9.57878 23.151 9.75704 23.1086 9.92682C23.0662 10.0966 22.9772 10.2512 22.8516 10.3731L18.4562 14.6588C18.3471 14.765 18.2655 14.8963 18.2186 15.0412C18.1717 15.1861 18.1609 15.3402 18.187 15.4902L19.2242 21.5451C19.2547 21.7189 19.2356 21.8978 19.1692 22.0613C19.1027 22.2248 18.9916 22.3662 18.8484 22.4694C18.7053 22.5727 18.536 22.6335 18.3599 22.645C18.1838 22.6564 18.0081 22.618 17.8528 22.5342L12.4373 19.6868C12.3025 19.6159 12.1525 19.5789 12.0002 19.5789C11.8479 19.5789 11.6979 19.6159 11.563 19.6868L6.1339 22.5428C5.9786 22.6266 5.80284 22.665 5.62674 22.6535C5.45064 22.6421 5.28134 22.5812 5.13821 22.478C4.99509 22.3748 4.88393 22.2333 4.81748 22.0698C4.75102 21.9064 4.73196 21.7275 4.76247 21.5537L5.79961 15.4988C5.82577 15.3488 5.81493 15.1946 5.76803 15.0498C5.72113 14.9049 5.63958 14.7736 5.53047 14.6674L1.1419 10.3782C1.01635 10.2563 0.927353 10.1018 0.88494 9.93196C0.842527 9.76218 0.848384 9.58392 0.90185 9.41728C0.955317 9.25064 1.05427 9.10225 1.18755 8.98884C1.32083 8.87542 1.48314 8.80149 1.65618 8.77538L7.73504 7.88566C7.88583 7.86355 8.02901 7.8052 8.15232 7.71563C8.27562 7.62606 8.37538 7.50794 8.44304 7.37138L11.1568 1.87024C11.2346 1.71304 11.3548 1.58072 11.5038 1.48821C11.6529 1.3957 11.8248 1.34668 12.0002 1.34668C12.1756 1.34668 12.3475 1.3957 12.4965 1.48821C12.6456 1.58072 12.7658 1.71304 12.8436 1.87024Z"
                                                fill="currentColor"></path>
                                        </svg>
                                        <p class="font-extralight text-sm text-[#333333]">5.0<span
                                                class="text-sm font-extralight text-[#757575] pl-1"> {{ product.new
                                                }}</span></p>
                                    </div>

                                </div>
                                <p
                                    class="m-auto flex items-center justify-center pb-2 text-[#7D3E1E] text-sm font-extralight">
                                    {{ product.offer }}</p>
                            </div>
                        </div>
                    </div>
                    <div class="grid1">
                        <div class=" h-full border py-[85px] px-6 flex items-center flex-col justify-center">
                            <div class="font-normal text-[22px] text-[#333333] pb-2" style="font-family: serif;">Get 50%
                                off your first order</div>
                            <p class="font-extralight text-sm text-[#333333] pb-4">Shop from more than 100,000
                                independent brands.</p>
                            <button class="mb-6 text-sm h-12 px-6 border bg-[#333333] text-[#fff] font-extralight">Sign up
                                for
                                free</button>
                            <p class="  font-extralight text-xs text-[#333333]">Maximum discount
                                $100. Offer ends 7 days after signup.</p>
                        </div>
                    </div>
                    <div class="grid2">
                        <div class="pt-4 pb-2 pl-4 flex flex-col">
                            <div class="font-serif font-[300px] text-[21px] text-[#333333] mb-4">Shop by brand values</div>
                            <div class="flex flex-row gap-2">
                                <div class="flex flex-col flex-grow">
                                    <div class="mb-2">
                                        <div
                                            class="w-fit py-2 px-4 rounded-[100px] border max-w-full flex items-center flex-row">
                                            <svg class="w-4 mr-2" focusable="false" viewBox="0 0 24 24"
                                                aria-labelledby="titleAccess-:r23:" role="img" fill="none">
                                                <g fill="currentColor" fill-rule="nonzero" stroke="currentColor"
                                                    stroke-width=".2">
                                                    <path
                                                        d="M7.01 3.522c.269-.403.557-.721.894-.97C8.412 2.183 9.018 2 9.809 2c.88 0 1.681.323 2.258.845.576.522.933 1.247.933 2.043 0 1.354-.733 2.69-1.832 4.016-1.075 1.296-2.482 2.57-3.89 3.844L7 13l-.279-.252C5.314 11.474 3.907 10.2 2.832 8.904 1.732 7.577 1 6.242 1 4.888c0-.796.357-1.521.933-2.043A3.363 3.363 0 0 1 4.191 2c1.358 0 2.125.509 2.804 1.522h.015zm1.383-.416c-.386.278-.709.716-1.031 1.309l-.347.628-.347-.628c-.63-1.137-1.246-1.707-2.453-1.707-.665 0-1.27.243-1.705.641A2.086 2.086 0 0 0 1.8 4.893c0 1.18.67 2.384 1.671 3.591C4.43 9.643 5.71 10.82 7.015 12c1.3-1.18 2.58-2.357 3.542-3.516 1.002-1.212 1.671-2.41 1.671-3.591 0-.602-.269-1.15-.708-1.544a2.544 2.544 0 0 0-1.706-.641c-.606 0-1.055.132-1.421.398zM14.01 19.096a.362.362 0 0 1-.356.37.363.363 0 0 1-.378-.348c-.023-.619-.535-.79-.668-.822H8.12a.3.3 0 0 1-.11-.018.637.637 0 0 1-.093-.027l-.009-.005c-.756-.235-2.121-.695-3.413-1.13-1.402-.469-2.716-.912-2.993-.989-.415-.112-.683.439-.683.439-.004.004-.004.013-.009.018-.193.339.06.677.148.786l8.73 4.752c.005.005.014.005.019.01.535.302 1.037.063 1.134.013a.434.434 0 0 1 .092-.045l6.48-2.096a.408.408 0 0 1 .13-.023h1.443c.203 0 .369.163.369.361a.366.366 0 0 1-.37.362h-1.387l-6.41 2.074c-.2.103-1.006.456-1.85-.023l-.01-.005-8.785-4.784a.397.397 0 0 1-.083-.063c0-.005-.784-.777-.305-1.654 0-.004.526-1.097 1.54-.822.328.09 1.638.529 3.035.999.766.257 1.555.524 2.21.74a2.025 2.025 0 0 1-.037-.388V16.769c.023-1.301 1.342-1.45 1.342-1.45.014 0 .032-.005.046-.005h3.376c.447-.198 2.748-1.201 3.99-1.418h.013c.553-.095 1.24-.127 1.863-.127.627 0 1.176.023 1.467.04.203.014.36.182.346.38a.364.364 0 0 1-.388.34c-.29-.019-.83-.041-1.42-.041-.581 0-1.222.031-1.739.117-.005 0-.01 0-.014.005-1.213.212-3.574 1.255-3.86 1.382a.354.354 0 0 1-.18.045H8.314c-.13.023-.669.154-.678.75 0 .14.018.253.05.348a.702.702 0 0 0 .42.416l.014.004c.01 0 .014.005.023.01l.01.004h4.487c.023 0 .046 0 .069.004.005 0 1.25.221 1.296 1.518l.005.005z">
                                                    </path>
                                                    <path
                                                        d="M23.208 13h-3.066a.08.08 0 0 0-.057.024.088.088 0 0 0-.026.063v9.043a.08.08 0 0 0 .026.062l.009.01c.013.01.03.02.053.02h3.066c.022 0 .044-.01.057-.03l.009-.01a.11.11 0 0 0 .017-.057v-9.043a.096.096 0 0 0-.022-.063c-.017-.019-.035-.029-.057-.029l-.009.01zm-3.066-.77h3.066c.216 0 .414.097.559.256.145.158.233.37.233.605v9.044c0 .22-.08.427-.207.581-.009.01-.017.02-.022.03a.76.76 0 0 1-.558.254h-3.066a.76.76 0 0 1-.533-.226c-.008-.01-.017-.02-.026-.024a.906.906 0 0 1-.233-.61v-9.044c0-.235.088-.452.233-.61a.747.747 0 0 1 .554-.255z">
                                                    </path>
                                                </g>
                                            </svg>
                                            <p class="font-extralight text-sm TEXT-[#333333]">Gives back</p>
                                        </div>
                                    </div>
                                    <div class="mb-2">
                                        <div
                                            class=" w-fit py-2 px-4 rounded-[100px] border max-w-full flex items-center flex-row">
                                            <p class="font-extralight text-sm text-[#333333]">LGBTQ owned</p>
                                        </div>
                                    </div>
                                    <div class="mb-2">
                                        <div
                                            class=" w-fit py-2 px-4 rounded-[100px] border max-w-full flex items-center flex-row">
                                            <svg class="mr-2 w-4" focusable="false" viewBox="0 0 36 37"
                                                aria-labelledby="titleAccess-:r24:" role="img" fill="none">
                                                <path
                                                    d="M8.92696 24.1549C11.0399 22.0737 11.6109 19.2619 10.2022 17.8745C8.7936 16.487 5.93879 17.0494 3.82584 19.1306C1.71289 21.2117 1.14192 24.0235 2.55056 25.411C3.9592 26.7984 6.81401 26.236 8.92696 24.1549Z"
                                                    stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10"
                                                    stroke-linecap="round" stroke-linejoin="round"></path>
                                                <path
                                                    d="M16.4847 32.3293C18.5976 30.2482 19.1686 27.4363 17.76 26.0489C16.3513 24.6615 13.4965 25.2239 11.3836 27.305C9.27063 29.3861 8.69966 32.198 10.1083 33.5854C11.5169 34.9728 14.3717 34.4105 16.4847 32.3293Z"
                                                    stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10"
                                                    stroke-linecap="round" stroke-linejoin="round"></path>
                                                <path d="M10.7979 21.204L35 10.7785" stroke="currentColor"
                                                    stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                                <path d="M15.6383 25.2998L25.3192 1.09766" stroke="currentColor"
                                                    stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                            </svg>
                                            <p class="font-extralight text-sm text-[#333333]">Handmade</p>
                                        </div>
                                    </div>
                                    <div class="mb-2">
                                        <div
                                            class="w-fit py-2 px-4 rounded-[100px] border max-w-full flex items-center flex-row">
                                            <svg class="mr-2 w-4" focusable="false" viewBox="0 0 31 40"
                                                aria-labelledby="titleAccess-:r25:" role="img" fill="none">
                                                <path
                                                    d="M1.03203 1C1.03203 1 -0.244364 15.4456 13.3173 15.8537C13.3173 15.8537 17.2263 3.04034 1.03203 1Z"
                                                    stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10"
                                                    stroke-linecap="round" stroke-linejoin="round"></path>
                                                <path d="M1 1L15.1463 17.9756" stroke="currentColor" stroke-width="1.5"
                                                    stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round">
                                                </path>
                                                <path
                                                    d="M29.968 1C29.968 1 31.2444 15.4456 17.6827 15.8537C17.6827 15.8537 13.7737 3.04034 29.968 1Z"
                                                    stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10"
                                                    stroke-linecap="round" stroke-linejoin="round"></path>
                                                <path d="M30 1L15.1464 18.0913V22.9268" stroke="currentColor"
                                                    stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                                <path d="M4.53662 22.9277H26.4634L25.7326 27.879H5.75478L4.53662 22.9277Z"
                                                    stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10"
                                                    stroke-linecap="round" stroke-linejoin="round"></path>
                                                <path d="M7.36584 27.8789L9.15275 39.196H22.4733L24.3415 27.8789"
                                                    stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10"
                                                    stroke-linecap="round" stroke-linejoin="round"></path>
                                            </svg>
                                            <p class="font-extralight text-sm text-[#333333]">Eco-friendly</p>
                                        </div>
                                    </div>
                                    <div class="mb-2">
                                        <div
                                            class="w-fit py-2 px-4 rounded-[100px] border max-w-full flex items-center flex-row">
                                            <svg class="mr-2 w-4" focusable="false" viewBox="0 0 36 33"
                                                aria-labelledby="titleAccess-:r26:" role="img" fill="none">
                                                <path
                                                    d="M36 5.92431C36 5.79622 35.9606 5.66012 35.8738 5.55604L31.639 0.224163C31.5286 0.0800582 31.3551 0 31.1737 0H4.8184C4.64491 0 4.47141 0.0800582 4.36101 0.224163L0.126177 5.55604C0.0394304 5.66012 0 5.79622 0 5.92431V5.93231V12.393C0 13.77 0.693976 14.9789 1.74283 15.6834V32.3996C1.74283 32.7278 2.01095 33 2.33428 33H13.8322H22.1678H33.6657C33.989 33 34.2572 32.7278 34.2572 32.3996V15.6834C35.306 14.9709 36 13.762 36 12.393V5.92431ZM5.1023 1.20087H30.8898L34.1704 5.33188H28.453H28.382H21.4344H14.4867H7.5391H1.82169L5.1023 1.20087ZM27.7906 6.53275V12.393C27.7906 13.9141 26.5761 15.147 25.0778 15.147H24.7465C23.2482 15.147 22.0337 13.9141 22.0337 12.393V6.53275H27.7906ZM20.8429 6.53275V12.393C20.8429 13.9141 19.6285 15.147 18.1301 15.147H17.7989C16.3005 15.147 15.0861 13.9141 15.0861 12.393V6.53275H20.8429ZM13.8953 6.53275V12.393C13.8953 13.9141 12.6808 15.147 11.1825 15.147H10.8513C9.3529 15.147 8.13844 13.9141 8.13844 12.393V6.53275H13.8953ZM1.18291 12.393V6.53275H6.94765V12.393C6.94765 13.9141 5.73319 15.147 4.23483 15.147H3.89573C2.39737 15.147 1.18291 13.9061 1.18291 12.393ZM21.5763 31.7991H14.4237V20.3748H21.5763V31.7991ZM33.0743 31.7991H22.7593V19.7744C22.7593 19.4461 22.4911 19.1739 22.1678 19.1739H13.8322C13.5089 19.1739 13.2407 19.4461 13.2407 19.7744V31.7991H2.92574V16.2038C3.24118 16.2838 3.56451 16.3399 3.89573 16.3399H4.22694C5.63067 16.3399 6.84513 15.5793 7.53122 14.4505C8.21731 15.5793 9.43965 16.3399 10.8355 16.3399H11.1667C12.5704 16.3399 13.7849 15.5793 14.471 14.4505C15.1571 15.5793 16.3794 16.3399 17.7752 16.3399H18.1065C19.5102 16.3399 20.7246 15.5793 21.4107 14.4505C22.0968 15.5793 23.3192 16.3399 24.715 16.3399H25.0462C26.4736 16.3399 27.7117 15.5473 28.3899 14.3865C29.0681 15.5473 30.3062 16.3399 31.7336 16.3399H32.0648C32.4039 16.3399 32.7273 16.2838 33.0348 16.2038V31.7991H33.0743ZM34.8171 12.393C34.8171 13.9141 33.6026 15.147 32.1043 15.147H31.7731C30.2747 15.147 29.0602 13.9141 29.0602 12.393V6.53275H34.825V12.393H34.8171ZM19.1001 25.7948C19.1001 25.4265 19.3919 25.1223 19.7625 25.1223C20.1332 25.1223 20.425 25.4185 20.425 25.7948C20.425 26.171 20.1332 26.4672 19.7625 26.4672C19.3919 26.4672 19.1001 26.163 19.1001 25.7948Z"
                                                    fill="currentColor"></path>
                                            </svg>
                                            <div class="_1jjg2vn2i _1jjg2vn5 _1jjg2vnu _1jjg2vn1j"
                                                style="--_1jjg2vn0: 8px;"></div>
                                            <p class="font-extralight text-sm text-[#333333]">Not on Amazon</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="flex flex-col flex-grow">
                                    <div class="mb-2">
                                        <div
                                            class=" w-fit py-2 px-4 rounded-[100px] border max-w-full flex items-center flex-row">
                                            <svg class="mr-2 w-4" focusable="false" viewBox="0 0 50 50"
                                                aria-labelledby="titleAccess-:r27:" role="img" fill="none">
                                                <path stroke="currentColor"
                                                    d="M33.28 37.34h-7.53v-10.1a11.91 11.91 0 1 0-1.5 0v10.1h-7.53a.75.75 0 1 0 0 1.5h7.53v6.83a.75.75 0 0 0 1.5 0v-6.83h7.53a.75.75 0 0 0 0-1.5zM14.59 15.43A10.41 10.41 0 1 1 25 25.78a10.39 10.39 0 0 1-10.41-10.35z">
                                                </path>
                                            </svg>
                                            <p class="font-extralight text-sm text-[#333333]">Women owned</p>
                                        </div>
                                    </div>
                                    <div>
                                        <div
                                            class=" w-fit py-2 px-4 rounded-[100px] border max-w-full flex items-center flex-row">
                                            <svg class="mr-2 w-4" focusable="false" viewBox="0 0 24 24"
                                                aria-labelledby="titleAccess-:r28:" role="img" fill="none">
                                                <path d="M21 18.7715H18.2443V12.3432V11.202H21V18.7715Z"
                                                    stroke="currentColor" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                                <path
                                                    d="M18.2439 12.6474C17.8995 12.6474 17.555 12.6474 17.1723 12.6474C16.5982 12.6474 15.9858 12.6474 15.4117 12.7235C14.3784 12.8756 13.4215 13.218 12.4265 13.4843C12.2351 13.5223 12.0437 13.5984 11.8524 13.5984H9.05844C8.59916 13.5984 8.17816 13.9787 8.17816 14.4732C8.17816 15.0058 8.59916 15.4242 9.13498 15.4242C9.51771 15.4242 9.90044 15.4242 10.2832 15.4242C10.819 15.4242 11.3548 15.4242 11.8906 15.4242C12.3116 15.4242 12.8092 15.5002 13.1154 15.8045"
                                                    stroke="currentColor" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                                <path
                                                    d="M9.13504 15.424C7.98685 15.3099 6.83867 15.0056 5.8053 14.5872C5.30775 14.397 4.8102 14.1688 4.31266 13.9025C4.08302 13.7884 3.85338 13.6743 3.58547 13.7503C3.39411 13.7884 3.20274 13.9025 3.1262 14.0546C2.85829 14.4731 3.04965 14.9675 3.39411 15.2718C3.39411 15.2718 5.61393 17.44 8.98195 18.0106C9.63259 18.1247 10.245 18.2007 10.8956 18.2007C11.7759 18.2007 12.6179 18.0486 13.4982 17.8964C14.034 17.7823 14.5698 17.7063 15.1056 17.5921C15.6032 17.478 16.1007 17.2878 16.6365 17.2878H18.2823"
                                                    stroke="currentColor" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                                <path
                                                    d="M13.7282 13.0274C13.7282 13.0274 13.2306 12.3427 12.3503 11.658C10.7811 10.4028 8.48477 10.7451 7.33659 12.3427C6.95386 12.8752 6.6094 13.5219 6.34149 14.3967"
                                                    stroke="currentColor" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                                <path
                                                    d="M10.1687 10.8977C10.1687 10.8977 9.67117 4.8878 14.1108 4.8878C14.1108 4.8878 13.996 8.34923 10.3984 8.38726"
                                                    stroke="currentColor" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                                <path
                                                    d="M10.3214 8.31115C10.3214 8.31115 10.7424 4.77365 7.14479 3.1C7.14479 3.1 6.49415 6.90376 10.1683 8.38723"
                                                    stroke="currentColor" stroke-miterlimit="10" stroke-linecap="round"
                                                    stroke-linejoin="round"></path>
                                            </svg>
                                            <p class="font-extralight text-sm text-[#333333]">Organic</p>
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
<script>
import data from './data.json'
export default {
    name: 'product-list',
    data() {
        return {
            productdata: data
        }
    },
}
</script>
<style>
.previous {
    transform: rotateZ(180deg);
}

.next {
    transform: rotateZ(0deg);
}

.grid1 {
    grid-area: 3 / 3 / span 1 / span 2;
}

.grid2 {
    grid-area: 6 / 3 / span 1 / span 2;
}
</style>