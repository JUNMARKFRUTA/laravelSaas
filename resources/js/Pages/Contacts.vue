<template>
    <nav class="bg-indigo-300">
        <div class="max-w-7xl mx-auto">
            <div class="flex justify-between">
                <div class="flex">  
                    <div>
                        <a href="/dashboard" class="flex items-center text-olive-500 hover:text-olive-600 py-4 px-3 transition duration-300">
                            <svg version="1.0" xmlns="http://www.w3.org/2000/svg" width="250 pt" height="40.000000pt" viewBox="0 0 350.000000 144.000000 " preserveAspectRatio="xMidYMid meet">

                   <g transform="translate(0.000000,144.000000) scale(0.100000,-0.100000)"
                 fill="#000000" stroke="none"> <path d="M2706 944 c-32 -31 -8 -84 38 -84 30 0 46 18 46 52 0 43 -53 64 -84 32z"/> <path d="M587 932 c-38 -42 -8 -102 51 -102 33 0 62 29 62 62 0 49 -80 77-113 40z"/><path d="M887 932 c-38 -42 -8 -102 51 -102 33 0 62 29 62 62 0 49 -80 77-113 40z"/><path d="M1210 922 c0 -4 22 -97 49 -207 l48 -200 45 -3 46 -3 48 142 c55 164 44 167 111 -29 l38 -113 45 3 44 3 48 195 c26 107 47 201 48 208 0 9 -12 12 -42 10 l-43 -3 -26 -138 c-15 -76 -29 -141 -32 -143 -2 -2 -26 60 -54 138 l-49 143 -35 3 -36 3 -48 -138 c-26 -76 -51 -141 -54 -145 -4 -5 -20 57 -35 137 l-28 145 -44 0 c-24 0 -44 -3 -44 -8z"/><path d="M2385 710 l0 -200 38 0 37 0 0 75 c0 41 3 75 8 75 4 0 30 -34 57 -75 l50 -74 48 -1 48 0 -61 82 c-49 68 -57 84 -47 97 6 9 31 40 56 69 l43 52 -48 0 c-48 0 -50 -2 -94 -60 -24 -33 -48 -60 -52 -60 -5 0 -8 50 -8 110 l0 110 -37 0 -38 0 0 -200z"/><path d="M2841 758 c0 -91 5 -167 12 -188 15 -44 65 -72 122 -68 37 3 40 5 43 36 3 30 1 32 -27 32 -51 0 -71 29 -71 105 l0 65 45 0 c45 0 45 0 45 35 0 32 -2 35 -29 35 -52 0 -61 8 -61 56 l0 44 -40 0 -40 0 1 -152z"/> <path d="M1849 797 c-43 -29 -69 -80 -69 -137 0 -98 62 -160 160 -160 103 0 164 67 158 171 -7 98 -64 149 -166 149 -34 0 -59 -7 -83 -23z m146 -72 c56 -55 18 -155 -59 -155 -45 0 -76 37 -76 92 0 49 35 88 80 88 19 0 40 -9 55 -25z"/> <path d="M2280 809 c-14 -5 -31 -17 -37 -26 -12 -15 -13 -15 -13 5 0 19 -6 22 -40 22 l-40 0 0 -150 0 -150 40 0 40 0 0 88 c0 105 12 129 71 138 39 7 40 8 37 43 -3 39 -17 46 -58 30z"/><path d="M2700 660 l0 -150 40 0 40 0 0 150 0 150 -40 0 -40 0 0 -150z"/> <path d="M557 759 c-41 -22 -76 -81 -77 -129 0 -43 42 -112 80 -132 41 -22 101 -23 138 -4 15 8 68 57 118 110 71 76 95 96 117 96 36 0 67 -33 67 -70 0 -59 -60 -88 -109 -54 -22 16 -24 15 -53 -13 l-30 -30 32 -23 c65 -47 153 -36 209 24 37 39 41 128 9 176 -43 64 -124 87 -192 55 -18 -9 -68 -56 -112 -106 -43 -50 -90 -93 -103 -96 -58 -14 -109 53 -78 101 23 35 63 44 101 22 29 -17 30 -16 54 8 22 21 24 27 12 41 -39 47 -120 58 -183 24z"/>
                     </g>
                        </svg>
                        </a>
                    </div>  
                 </div>
                 <div class="hidden lg:flex items-center uppercase space-x-20 text-olive-500 font-semibold">
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
            <a href="/about us" class="block py-1 text-md hover:text-gray-900 text-olive-500 transition duration-300">about us</a> 
            <a href="/contacts" class="block py-1 text-md hover:text-gray-900 text-olive-500 transition duration-300">contacts</a> 
            <a href="/services" class="block py-1 text-md hover:text-gray-900 text-olive-500 transition duration-300">services</a>
            <a :href="route('login')" class="py-2 px-2 block rounded-full bg-olive-400 hover:bg-olive-600 text-white  shadow-lg shadow-sm transition duration-300">login</a>  
            <a :href="route('register')" class="py-2 px-2 block mt-1 rounded-full bg-olive-400 hover:bg-olive-600 text-white shadow-lg shadow-sm transition duration-300 mb-2">register</a>  
        </div>
    </nav>
            
  <div style="background-image: url('/images/cool-background.png');">
  <div class="splide lg:ml-10 lg:mr-10" id="card-slider">
	        <div class="splide__track">
		        <ul class="splide__list">
			        <li class="splide__slide  rounded">
                        <div class="text-xl font-semibold mt-20 py-5 ml-10 px-5 mr-10 text-black">
                            <p class="">Get In Touch</p><br><p>
                                Want to outsource your IT? Got a burning IT question? Is your server room on fire? Give us a call! We have local, certified IT professionals standing by to help with any IT problem or question.
                           </p >
                           <p>SALES INQUIRIES NUMBER:(091-123-234-123)</p>
                        </div>
                    </li>
                    
			        <li class="splide__slide rounded"> 
                        <div class="text-xl font-semibold mt-20 py-5 ml-10 px-5 mr-10 text-black">
                          Our Locations <br><br>
                           We’re bringing the WorkIT Way to organizations across the West! We have offices in Malaybalay,City Bukidnon and beyond with more on the way.  Curious to meet the tech experts behind the magic? Stop by and say hi! Or reach us by phone: (091-123-234-123)
                        </div>
                    </li>
                    
		        </ul>
	        </div>  
        </div>
        
    </div>
  


</template>
<script>

    export default {
    mounted(){
            const btn = document.querySelector('button.mobile-menu-button')
            const menu = document.querySelector('.mobile-menu')
            btn.addEventListener("click",()=>{
            menu.classList.toggle("hidden");
            });
            new Splide( '#card-slider',{
                type:'loop',
                speed: 600,
                perPage:1
    
                
            } ).mount();
        }
}
</script>