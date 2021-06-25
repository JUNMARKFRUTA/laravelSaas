<template>
    <nav class="">
        <div class="max-w-7xl mx-auto ">
            <div class="flex justify-between bg-gray-500">
                <div class="flex ">  
                    <div>
                        <a href="/dashboard" class="flex items-center bg-gray-500 text-olive-500 hover:text-olive-600 py-4 px-3 transition duration-300">
                
                 <svg version="1.0" xmlns="http://www.w3.org/2000/svg" width="250 pt" height="40.000000pt" viewBox="0 0 350.000000 144.000000 " preserveAspectRatio="xMidYMid meet">
                   <g transform="translate(0.000000,144.000000) scale(0.100000,-0.100000)"
                 fill="#000000" stroke="none"> <path d="M2706 944 c-32 -31 -8 -84 38 -84 30 0 46 18 46 52 0 43 -53 64 -84 32z"/> <path d="M587 932 c-38 -42 -8 -102 51 -102 33 0 62 29 62 62 0 49 -80 77-113 40z"/><path d="M887 932 c-38 -42 -8 -102 51 -102 33 0 62 29 62 62 0 49 -80 77-113 40z"/><path d="M1210 922 c0 -4 22 -97 49 -207 l48 -200 45 -3 46 -3 48 142 c55 164 44 167 111 -29 l38 -113 45 3 44 3 48 195 c26 107 47 201 48 208 0 9 -12 12 -42 10 l-43 -3 -26 -138 c-15 -76 -29 -141 -32 -143 -2 -2 -26 60 -54 138 l-49 143 -35 3 -36 3 -48 -138 c-26 -76 -51 -141 -54 -145 -4 -5 -20 57 -35 137 l-28 145 -44 0 c-24 0 -44 -3 -44 -8z"/><path d="M2385 710 l0 -200 38 0 37 0 0 75 c0 41 3 75 8 75 4 0 30 -34 57 -75 l50 -74 48 -1 48 0 -61 82 c-49 68 -57 84 -47 97 6 9 31 40 56 69 l43 52 -48 0 c-48 0 -50 -2 -94 -60 -24 -33 -48 -60 -52 -60 -5 0 -8 50 -8 110 l0 110 -37 0 -38 0 0 -200z"/><path d="M2841 758 c0 -91 5 -167 12 -188 15 -44 65 -72 122 -68 37 3 40 5 43 36 3 30 1 32 -27 32 -51 0 -71 29 -71 105 l0 65 45 0 c45 0 45 0 45 35 0 32 -2 35 -29 35 -52 0 -61 8 -61 56 l0 44 -40 0 -40 0 1 -152z"/> <path d="M1849 797 c-43 -29 -69 -80 -69 -137 0 -98 62 -160 160 -160 103 0 164 67 158 171 -7 98 -64 149 -166 149 -34 0 -59 -7 -83 -23z m146 -72 c56 -55 18 -155 -59 -155 -45 0 -76 37 -76 92 0 49 35 88 80 88 19 0 40 -9 55 -25z"/> <path d="M2280 809 c-14 -5 -31 -17 -37 -26 -12 -15 -13 -15 -13 5 0 19 -6 22 -40 22 l-40 0 0 -150 0 -150 40 0 40 0 0 88 c0 105 12 129 71 138 39 7 40 8 37 43 -3 39 -17 46 -58 30z"/><path d="M2700 660 l0 -150 40 0 40 0 0 150 0 150 -40 0 -40 0 0 -150z"/> <path d="M557 759 c-41 -22 -76 -81 -77 -129 0 -43 42 -112 80 -132 41 -22 101 -23 138 -4 15 8 68 57 118 110 71 76 95 96 117 96 36 0 67 -33 67 -70 0 -59 -60 -88 -109 -54 -22 16 -24 15 -53 -13 l-30 -30 32 -23 c65 -47 153 -36 209 24 37 39 41 128 9 176 -43 64 -124 87 -192 55 -18 -9 -68 -56 -112 -106 -43 -50 -90 -93 -103 -96 -58 -14 -109 53 -78 101 23 35 63 44 101 22 29 -17 30 -16 54 8 22 21 24 27 12 41 -39 47 -120 58 -183 24z"/>
                </g>
                        </svg>
                          
                        </a>
                    </div>  
                </div>
                <div class=" hidden lg:flex items-center uppercase space-x-20 text-yellow-500 font-bold ">
                     <div>
                        <a href="/welcome" class="hover:text-gray-900 transition duration-300">home</a>    
                    </div>
                    <div>
                        <a href="/aboutus" class="hover:text-gray-900 transition duration-300">about us</a>    
                    </div>
                    <div>
                        <a href="/contacts" class="hover:text-gray-900 transition duration-300">contacts</a>  
                    </div>
                    <div>
                        <a href="/services" class="hover:text-gray-900 transition duration-300">services</a>
                    </div>
                
                    <div v-if="!$page.props.user">
                        <a :href="route('login')" class="rounded-full bg-olive-400 hover:bg-olive-600 text-white px-6 p-2 shadow-lg shadow-sm transition duration-300">login</a>  
                    </div>
                    <div v-if="!$page.props.user">
                        <a :href="route('register')" class="rounded-full bg-olive-400 hover:bg-olive-600 text-white px-6 p-2 shadow-lg shadow-sm transition duration-300">register</a>  
                    </div>
                </div>
                <div class="lg:hidden flex items-center">
                    <button class="mobile-menu-button">
                       <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-black bg-gray-100" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                    </button>
                </div>
            </div>       
            
        </div>
        <div class="mobile-menu lg:hidden hidden ml-2 uppercase">
            <a href="/welcome" class="block py-1 text-md hover:text-gray-900 text-olive-500 transition duration-300">home</a> 
            <a href="/about us" class="block py-1 text-md hover:text-gray-900 text-olive-500 transition duration-300">about us</a> 
            <a href="/contacts" class="block py-1 text-md hover:text-gray-900 text-olive-500 transition duration-300">contacts</a> 
            <a href="/careers" class="block py-1 text-md hover:text-gray-900 text-olive-500 transition duration-300">careers</a>
            <a :href="route('login')" class="py-2 px-2 block rounded-full bg-olive-400 hover:bg-olive-600 text-white  shadow-lg shadow-sm transition duration-300">login</a>  
            <a :href="route('register')" class="py-2 px-2 block mt-1 rounded-full bg-olive-400 hover:bg-olive-600 text-white shadow-lg shadow-sm transition duration-300 mb-2">register</a>  
        </div>
    </nav>
  
       
  <div style="background-image: url('/images/cool-background.png');">
<section class="w-full px-3 antialiased lg:px-6">
    <div class="mx-auto max-w-7xl">
        <nav class="flex items-center w-full h-24 select-none" x-data="{ showMenu: false }">
            <div class="relative flex flex-wrap items-center justify-between w-full h-24 mx-auto font-medium md:justify-center">
                
                <div class="fixed top-0 left-0 z-40 items-center hidden w-full h-full p-3 text-xl bg-gray-900 bg-opacity-50 md:text-sm lg:text-base md:w-3/4 md:bg-transparent md:p-0 md:relative md:flex" :class="{'flex': showMenu, 'hidden': !showMenu }">
                    <div class="flex-col w-full h-auto h-full overflow-hidden bg-white rounded-lg select-none md:bg-transparent md:rounded-none md:relative md:flex md:flex-row md:overflow-auto">
                        <div class="flex flex-col items-center justify-center w-full h-full mt-12 text-center text-indigo-700 md:text-indigo-200 md:w-2/3 md:mt-0 md:flex-row md:items-center">
                            <a href="#" class="inline-block px-4 py-2 mx-2 font-medium text-left text-indigo-700 md:text-white md:px-0 lg:mx-3 md:text-center"></a>
                            <a href="#" class="inline-block px-0 px-4 py-2 mx-2 font-medium text-left md:px-0 hover:text-indigo-800 md:hover:text-white lg:mx-3 md:text-center"></a>
                            <a href="#" class="inline-block px-0 px-4 py-2 mx-2 font-medium text-left md:px-0 hover:text-indigo-800 md:hover:text-white lg:mx-3 md:text-center"></a>
                            <a href="#" class="inline-block px-0 px-4 py-2 mx-2 font-medium text-left md:px-0 hover:text-indigo-800 md:hover:text-white lg:mx-3 md:text-center"></a>
                        </div>
                       
                    </div>
                </div>
                <div @click="showMenu = !showMenu" class="absolute right-0 z-50 flex flex-col items-end w-10 h-10 p-2 mr-4 rounded-full cursor-pointer md:hidden hover:bg-gray-900 hover:bg-opacity-10" :class="{ 'text-gray-400': showMenu, 'text-gray-100': !showMenu }">
                    <svg class="w-6 h-6" x-show="!showMenu" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor" x-cloak="">
                        <path d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                    <svg class="w-6 h-6" x-show="showMenu" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" x-cloak="">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                    </svg>
                </div>
            </div>
        </nav>
        <div class="container py-32 mx-auto text-center sm:px-4">

            <h1 class="text-4xlnpm run hue-rotate- font-extrabold leading-10 tracking-tight text-red-200 sm:text-5xl sm:leading-none md:text-6xl xl:text-7xl"><span class="block">Let's Get Start Designing</span> <span class="relative inline-block mt-3 text-transparent text-black"></span></h1>
   
            <div class="relative flex items-center max-w-md mx-auto mt-12 overflow-hidden text-center rounded-full">
                   <a href="#_" class="inline-flex items-center justify-center w-full px-5 py-4 mt-6 ml-0 font-sans text-base leading-none text-white no-underline bg-indigo-600 border border-indigo-600 border-solid rounded cursor-pointer md:w-auto lg:mt-0 hover:bg-indigo-700 hover:border-indigo-700 hover:text-white focus-within:bg-indigo-700 focus-within:border-indigo-700 focus-within:text-white sm:text-lg lg:ml-6 md:text-xl">
                Get Started
                <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5 ml-2" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <line x1="5" y1="12" x2="19" y2="12"></line>
                    <polyline points="12 5 19 12 12 19"></polyline>
                </svg>
            </a>
        </div>
          
          
        </div>
    </div>
</section>
</div>
     

<!-- Section 3 -->
<section class="flex items-center justify-center py-16 bg-gray-100 min-w-screen">
    <div class="max-w-6xl px-12 mx-auto bg-gray-100 md:px-16 xl:px-10">
        <div class="flex flex-col items-center lg:flex-row">
            <div class="flex flex-col items-start justify-center w-full h-full pr-8 mb-10 lg:mb-0 lg:w-1/2">
                <p class="mb-2 text-base font-medium tracking-tight text-indigo-500 uppercase">Our customers love our product</p>
                <h2 class="text-4xl font-extrabold leading-10 tracking-tight text-gray-900 sm:text-5xl sm:leading-none md:text-6xl lg:text-5xl xl:text-6xl">Testimonials</h2>
                <p class="my-6 text-lg text-gray-600">Don't just take our word for it, read from our extensive list of case studies and customer testimonials.</p>
                <a href="#_" class="flex items-center justify-center px-8 py-3 text-base font-medium leading-6 text-white transition duration-150 ease-in-out bg-indigo-600 border border-transparent rounded-md shadow hover:bg-indigo-500 focus:outline-none focus:border-indigo-700 focus:shadow-outline-indigo md:py-4 md:text-lg md:px-10">View Case Studies</a>
            </div>
            <div class="w-full lg:w-1/2">
                <blockquote class="flex items-center justify-between w-full col-span-1 p-6 bg-white rounded-lg shadow">
                    <div class="flex flex-col pr-8">
                        <div class="relative pl-12">
                            <svg class="absolute left-0 w-10 h-10 text-indigo-500 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 125">
                                <path d="M30.7 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2C12.7 83.1 5 72.6 5 61.5c0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S30.7 31.6 30.7 42zM82.4 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2-11.8 0-19.5-10.5-19.5-21.6 0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S82.4 31.6 82.4 42z"></path>
                            </svg>
                            <p class="mt-2 text-sm text-gray-600 sm:text-base lg:text-sm xl:text-base">Awesome product! And the customer service is exceptionally well.</p>
                        </div>

                        <h3 class="pl-12 mt-3 text-sm font-medium leading-5 text-gray-800 truncate sm:text-base lg:text-sm lg:text-base">
                            Jezamyn Oyao
                            <span class="mt-1 text-sm leading-5 text-gray-500 truncate">- CEO SomeCompany</span>
                        </h3>
                    </div>
                    <img class="flex-shrink-0 w-20 h-20 bg-gray-300 rounded-full xl:w-24 xl:h-24" src="/images/oyao.jpg" alt="">
                </blockquote>
                <blockquote class="flex items-center justify-between w-full col-span-1 p-6 mt-4 bg-white rounded-lg shadow">
                    <div class="flex flex-col pr-10">
                        <div class="relative pl-12">
                            <svg class="absolute left-0 w-10 h-10 text-indigo-500 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 125">
                                <path d="M30.7 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2C12.7 83.1 5 72.6 5 61.5c0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S30.7 31.6 30.7 42zM82.4 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2-11.8 0-19.5-10.5-19.5-21.6 0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S82.4 31.6 82.4 42z"></path>
                            </svg>
                            <p class="mt-2 text-sm text-gray-600 sm:text-base lg:text-sm xl:text-base">I can't express enough, how amazing this service has been for my company.</p>
                        </div>
                        <h3 class="pl-12 mt-3 text-sm font-medium leading-5 text-gray-800 truncate sm:text-base lg:text-sm lg:text-base">
                            Jun Mark Fruta
                            <span class="mt-1 text-sm leading-5 text-gray-500 truncate">- CEO SomeCompany</span>
                        </h3>
                        <p class="mt-1 text-sm leading-5 text-gray-500 truncate"></p>
                    </div>
                    <img class="flex-shrink-0 w-24 h-24 bg-gray-300 rounded-full" src="/images/ako.jpg" alt="">
                </blockquote>
                <blockquote class="flex items-center justify-between w-full col-span-1 p-6 mt-4 bg-white rounded-lg shadow">
                    <div class="flex flex-col pr-10">
                        <div class="relative pl-12">
                            <svg class="absolute left-0 w-10 h-10 text-indigo-500 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 125">
                                <path d="M30.7 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2C12.7 83.1 5 72.6 5 61.5c0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S30.7 31.6 30.7 42zM82.4 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2-11.8 0-19.5-10.5-19.5-21.6 0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S82.4 31.6 82.4 42z"></path>
                            </svg>
                            <p class="mt-2 text-sm text-gray-600 sm:text-base lg:text-sm xl:text-base">I can't express enough, how amazing this service has been for my company.</p>
                        </div>

                        <h3 class="pl-12 mt-3 text-sm font-medium leading-5 text-gray-800 truncate sm:text-base lg:text-sm lg:text-base">
                            Jayson Golosino
                            <span class="mt-1 text-sm leading-5 text-gray-500 truncate">- CEO SomeCompany</span>
                        </h3>
                        <p class="mt-1 text-sm leading-5 text-gray-500 truncate"></p>
                    </div>
                    <img class="flex-shrink-0 w-24 h-24 bg-gray-300 rounded-full" src="/images/jayson.jpg" alt="">
                </blockquote>
            </div>
        </div>
    </div>
</section>

<section class="bg-white pt-7 pb-14">
    <div class="container px-8 mx-auto sm:px-12 lg:px-20">
        <h1 class="text-sm font-bold tracking-wide text-center text-gray-800 uppercase mb-7">Trusted by top-leading companies.</h1>
        <div class="flex grid items-center justify-center grid-cols-4 grid-cols-12 gap-y-8">
            <div class="flex items-center justify-center col-span-6 sm:col-span-4 md:col-span-3 xl:col-span-2">
                <img src="https://cdn.devdojo.com/tails/images/disney-plus.svg" alt="Disney Plus" class="block object-contain h-12">
            </div>
            <div class="flex items-center justify-center col-span-6 sm:col-span-4 md:col-span-3 xl:col-span-2">
                <img src="https://cdn.devdojo.com/tails/images/google.svg" alt="Google" class="block object-contain h-9">
            </div>
            <div class="flex items-center justify-center col-span-6 sm:col-span-4 md:col-span-3 xl:col-span-2">
                <img src="https://cdn.devdojo.com/tails/images/hubspot.svg" alt="Hubspot" class="block object-contain h-9">
            </div>
            <div class="flex items-center justify-center col-span-6 sm:col-span-4 md:col-span-3 xl:col-span-2">
                <img src="https://cdn.devdojo.com/tails/images/youtube.svg" alt="Youtube" class="block object-contain h-7 lg:h-8">
            </div>
            <div class="flex items-center justify-center col-span-6 sm:col-span-4 md:col-span-6 xl:col-span-2">
                <img src="https://cdn.devdojo.com/tails/images/slack.svg" alt="Slack" class="block object-contain h-9">
            </div>
            <div class="flex items-center justify-center col-span-6 sm:col-span-4 md:col-span-6 xl:col-span-2">
                <img src="https://cdn.devdojo.com/tails/images/shopify.svg" alt="Shopify" class="block object-contain h-9">
            </div>
        </div>
    </div>
</section>

</template>


