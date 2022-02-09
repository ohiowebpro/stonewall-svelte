<script lang="ts">
    import { page } from '$app/stores';
    import logo from './logo.svg';
</script>

<header class="text-white fixed top-0 left-0 right-0 z-20 py-3">



    <nav class="px-10 py-2.50 uppercase ">
        <div class="container flex flex-wrap justify-between items-center mx-auto">
            <a href="/" class="flex">
                <img src={logo} alt="Stonewall Group Logo" class="w-60 brightness-0 invert my-6" />
            </a>
            <button data-collapse-toggle="mobile-menu" type="button" class="inline-flex items-center p-2 ml-3 text-sm text-white rounded-lg md:hidden hover:text-stone-400 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 " aria-controls="mobile-menu-2" aria-expanded="false">
                <span class="sr-only">Open main menu</span>
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
                <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
            </button>
            <div class="hidden w-full md:block md:w-auto" id="mobile-menu">
                <ul class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium mr-10">
                    <li class:active={$page.url.pathname === '/work'}>
                        <a sveltekit:prefetch href="/work" class="block py-2 pr-4 pl-3 text-white md:p-0 dark:text-white" >Our Work</a>
                    </li>
                    <li class:active={$page.url.pathname === '/about'}>
                        <a sveltekit:prefetch href="/about" class="block py-2 pr-4 pl-3 text-white md:p-0 dark:text-white">About Us</a>
                    </li>
                    <li class:active={$page.url.pathname === '/contact'}>
                        <a sveltekit:prefetch href="/contact"  class="block py-2 pr-4 pl-3 text-white md:p-0 dark:text-white">Contact Us</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>





</header>