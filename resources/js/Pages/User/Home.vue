<template>
    <nav class="">
        <div class="max-w-7xl mx-auto">
            <div class="flex justify-between">
                <div class="flex">  
                    <div>
                        <a href="/dashboard" class="flex items-center text-olive-500 hover:text-olive-600 py-4 px-3 transition duration-300">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" viewBox="0 0 20 20" fill="currentColor">
                                <path fill-rule="evenodd" d="M6 6V5a3 3 0 013-3h2a3 3 0 013 3v1h2a2 2 0 012 2v3.57A22.952 22.952 0 0110 13a22.95 22.95 0 01-8-1.43V8a2 2 0 012-2h2zm2-1a1 1 0 011-1h2a1 1 0 011 1v1H8V5zm1 5a1 1 0 011-1h.01a1 1 0 110 2H10a1 1 0 01-1-1z" clip-rule="evenodd" />
                                <path d="M2 13.692V16a2 2 0 002 2h12a2 2 0 002-2v-2.308A24.974 24.974 0 0110 15c-2.796 0-5.487-.46-8-1.308z" />
                            </svg>
                            <span class="text-xl font-bold ">
                                WorkIT
                            </span>
                        </a>
                    </div>  
                </div>
                <div class="hidden lg:flex items-center uppercase space-x-20 text-yellow-500 font-semibold">
                     <div>
                        <a href="/home" class="hover:text-gray-900 transition duration-300">home</a>    
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
    
<section class="w-full px-3 antialiased bg-indigo-600 lg:px-6">
    <div class="mx-auto max-w-7xl">
        <nav class="flex items-center w-full h-24 select-none" x-data="{ showMenu: false }">
            <div class="relative flex flex-wrap items-center justify-between w-full h-24 mx-auto font-medium md:justify-center">
                <a href="#_" class="w-1/4 py-4 pl-6 pr-4 md:pl-4 md:py-0">
                    <span class="p-1 text-xl font-black leading-none text-white select-none"><span></span><span class="text-indigo-300">.</span></span>
                </a>
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

            <h1 class="text-4xl font-extrabold leading-10 tracking-tight text-black sm:text-5xl sm:leading-none md:text-6xl xl:text-7xl"><span class="block">Let's Get Start Designing</span> <span class="relative inline-block mt-3 text-transparent text-black"></span></h1>
            <div class="max-w-lg mx-auto mt-6 text-sm text-center text-indigo-200 md:mt-12 sm:text-base md:max-w-xl md:text-lg xl:text-xl">Design Websites with the Best Framework</div>
            <div class="relative flex items-center max-w-md mx-auto mt-12 overflow-hidden text-center rounded-full">
                <input type="text" name="email" placeholder="Email Address" class="w-full h-12 px-6 py-2 font-medium text-indigo-800 focus:outline-none">
                <span class="relative top-0 right-0 block">
                    <button type="button" class="inline-flex items-center w-32 h-12 px-8 text-base font-bold leading-6 text-white transition duration-150 ease-in-out bg-indigo-400 border border-transparent hover:bg-indigo-700 focus:outline-none active:bg-indigo-700">
                        Sign Up
                    </button>
                </span>
            </div>
            <div class="mt-8 text-sm text-indigo-300">By signing up, you agree to our terms and services.</div>
        </div>
    </div>
</section>
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
                    <img class="flex-shrink-0 w-20 h-20 bg-gray-300 rounded-full xl:w-24 xl:h-24" src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;auto=format&amp;fit=facearea&amp;facepad=4&amp;w=256&amp;h=256&amp;q=60" alt="">
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
                    <img class="flex-shrink-0 w-24 h-24 bg-gray-300 rounded-full" src="https://images.unsplash.com/photo-1527980965255-d3b416303d12?ixlib=rb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;aauto=format&amp;fit=facearea&amp;facepad=4&amp;w=256&amp;h=256&amp;q=60" alt="">
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
                    <img class="flex-shrink-0 w-24 h-24 bg-gray-300 rounded-full" src="https://images.unsplash.com/photo-1545167622-3a6ac756afa4?ixlib=rrb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;aauto=format&amp;fit=facearea&amp;facepad=4&amp;w=256&amp;h=256&amp;q=60" alt="">
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


