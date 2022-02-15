<script context="module" lang="ts">
    export const prerender = true;
    import image1 from './../img/macbook-screen.png';
    import image2 from './../img/samples.png';

    const images = [
        {path: '/src/img/samples.png', id: 'image1'},
        {path: '/src/img/samples.png', id: 'image2'},
        {path: '/src/img/samples.png', id: 'image3'},
        {path: '/src/img/samples.png', id: 'image4'},

    ]

</script>

<svelte:head>
    <title>Home</title>
</svelte:head>

<div class="text-white bg-no-repeat bg-cover bg-[url('https://picsum.photos/id/1/1600/900')] w-full aspect-video overflow-hidden relative z-0"  >
    <div class="swg-clip absolute left-0 top-0 bottom-0 right-1/2 bg-primary opacity-90"></div>
    <div class="container mx-auto relative h-full px-10  ">
        <h2 class="absolute bottom-10 uppercase text-3xl font-bold w-1/4">Discover What is Possible.</h2>
    </div>

</div>

<div class="container mx-auto px-6">
    <h1 class="text-center text-2xl py-20 mx-20 text-gray font-bold">We are a group of passionate, relentless, and connected people who use the power of creativity to solve our clients' problems.</h1>
</div>

<div class="container mx-auto px-6">
    <div class="grid grid-cols-12 gap-4 md:gap-6 mb-12">
        <div class="col-span-full md:col-span-5">
            <div class="opacity-60 hover:opacity-100 bg-ltgray bg-gradient-to-t from-ltgraybtm hover:bg-primary hover:from-primarygrad transition-all grid justify-items-center items-center h-full relative">
                <img src="{image1}" alt="a computer" class="" />
                <a href="test" class="text-black hover:text-white transition-colors font-bold text-4xl uppercase absolute top-0 bottom-0 left-0 right-0 group" ><span class="group-hover:top-3/4 absolute left-1/2 top-1/2 -translate-y-1/2 -translate-x-1/2 transition-all">Video</span></a>
            </div>
        </div>
        <div class="col-span-full md:col-span-7">
            <div class="opacity-60 hover:opacity-100 bg-ltgray bg-gradient-to-t from-ltgraybtm hover:bg-primary hover:from-primarygrad transition-all grid justify-items-center items-center h-full relative">
                <img src="{image1}" alt="a computer" class="" />
                <a href="test" class="text-black hover:text-white transition-colors font-bold text-4xl uppercase absolute top-0 bottom-0 left-0 right-0 group" ><span class="group-hover:top-3/4 absolute left-1/2 top-1/2 -translate-y-1/2 -translate-x-1/2 transition-all">Campaign</span></a>
            </div>
        </div>
        <div class="col-span-full">
            <div class="opacity-60 hover:opacity-100 bg-ltgray bg-gradient-to-t from-ltgraybtm hover:bg-primary hover:from-primarygrad transition-all grid justify-items-center items-center h-full relative">
                <img src="{image1}" alt="a computer" class="" />
                <a href="test" class="ftext-black hover:text-white transition-colors font-bold text-4xl uppercase absolute top-0 bottom-0 left-0 right-0 group" ><span class="group-hover:top-3/4 absolute left-1/2 top-1/2 -translate-y-1/2 -translate-x-1/2 transition-all">Web</span></a>
            </div>
        </div>
        <div class="col-span-full md:col-span-7">
            <div class="opacity-60 hover:opacity-100 bg-ltgray bg-gradient-to-t from-ltgraybtm hover:bg-primary hover:from-primarygrad transition-all grid justify-items-center items-center h-full relative">
                <img src="{image1}" alt="a computer" class="" />
                <a href="test" class=" text-center text-black hover:text-white transition-colors font-bold text-4xl uppercase absolute top-0 bottom-0 left-0 right-0 group" ><span class="group-hover:top-3/4 absolute left-1/2 top-1/2 -translate-y-1/2 -translate-x-1/2 transition-all">Brand<br />Identity</span></a>
            </div>
        </div>
        <div class="col-span-full md:col-span-5">
            <div class="opacity-60 hover:opacity-100 bg-ltgray bg-gradient-to-t from-ltgraybtm hover:bg-primary hover:from-primarygrad transition-all grid justify-items-center items-center h-full relative">
                <img src="{image1}" alt="a computer" class="" />
                <a href="test" class="ftext-black hover:text-white transition-colors font-bold text-4xl uppercase absolute top-0 bottom-0 left-0 right-0 group" ><span class="group-hover:top-3/4 absolute left-1/2 top-1/2 -translate-y-1/2 -translate-x-1/2 transition-all">Print</span></a>
            </div>
        </div>
    </div>
</div>

<div class="bg-ltgray relative">

    <div id="carousel-container" class="absolute right-0 h-full z-0">
        <div id="carousel-images">
            {#each images as image}
                <img src="{image.path}" alt="{image.id}" id="{image.id}" />
            {/each}
        </div>
    </div>
    <div class="container mx-auto relative z-10">

        <div class="w-5/12 py-28">
            <p class="my-20"><a href="/" class="text-2xl font-bold text-gray hover:text-black transition-colors flex group">Kitchen Cabinet Distributors<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 ml-3 group-hover:translate-x-6  transition-all" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd" />
                </svg>
            </a></p>
            <p class="my-20"><a href="/" class="text-2xl font-bold text-gray hover:text-black transition-colors flex group">OhioSE Economic Development<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 ml-3 group-hover:translate-x-6  transition-all" viewBox="0 0 20 20" fill="currentColor">
                <path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd" /></a></p>
            <p class="my-20"><a href="/" class="text-2xl font-bold text-gray hover:text-black transition-colors flex group">West Virginia Economic Development<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 ml-3 group-hover:translate-x-6  transition-all" viewBox="0 0 20 20" fill="currentColor">
                <path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd" /></a></p>
        </div>
    </div>

</div>





<h2>Header Level 2</h2>

<ol>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ol>

<blockquote><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus magna. Cras in mi at felis aliquet congue. Ut a est eget ligula molestie gravida. Curabitur massa. Donec eleifend, libero at sagittis mollis, tellus est malesuada tellus, at luctus turpis elit sit amet quam. Vivamus pretium ornare est.</p></blockquote>

<h3>Header Level 3</h3>

<ul>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ul>


<h1>HTML Ipsum Presents</h1>

<p><strong>Pellentesque habitant morbi tristique</strong> senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. <em>Aenean ultricies mi vitae est.</em> Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, <code>commodo vitae</code>, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. <a href="/">Donec non enim</a> in turpis pulvinar facilisis. Ut felis.</p>

<h2>Header Level 2</h2>

<ol>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ol>

<blockquote><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus magna. Cras in mi at felis aliquet congue. Ut a est eget ligula molestie gravida. Curabitur massa. Donec eleifend, libero at sagittis mollis, tellus est malesuada tellus, at luctus turpis elit sit amet quam. Vivamus pretium ornare est.</p></blockquote>

<h3>Header Level 3</h3>

<ul>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ul>



<h1>HTML Ipsum Presents</h1>

<p><strong>Pellentesque habitant morbi tristique</strong> senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. <em>Aenean ultricies mi vitae est.</em> Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, <code>commodo vitae</code>, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. <a href="/">Donec non enim</a> in turpis pulvinar facilisis. Ut felis.</p>

<h2>Header Level 2</h2>

<ol>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ol>

<blockquote><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus magna. Cras in mi at felis aliquet congue. Ut a est eget ligula molestie gravida. Curabitur massa. Donec eleifend, libero at sagittis mollis, tellus est malesuada tellus, at luctus turpis elit sit amet quam. Vivamus pretium ornare est.</p></blockquote>

<h3>Header Level 3</h3>

<ul>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ul>



<h1>HTML Ipsum Presents</h1>

<p><strong>Pellentesque habitant morbi tristique</strong> senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. <em>Aenean ultricies mi vitae est.</em> Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, <code>commodo vitae</code>, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. <a href="/">Donec non enim</a> in turpis pulvinar facilisis. Ut felis.</p>

<h2>Header Level 2</h2>

<ol>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ol>

<blockquote><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus magna. Cras in mi at felis aliquet congue. Ut a est eget ligula molestie gravida. Curabitur massa. Donec eleifend, libero at sagittis mollis, tellus est malesuada tellus, at luctus turpis elit sit amet quam. Vivamus pretium ornare est.</p></blockquote>

<h3>Header Level 3</h3>

<ul>
    <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
    <li>Aliquam tincidunt mauris eu risus.</li>
</ul>

<style>
    #carousel-container {
        width: 100%;
        position: relative;
        display: flex;
        flex-direction: column;
        overflow-x: hidden;
    }
    #carousel-images {
        display: flex;
        justify-content: center;
        flex-wrap: nowrap;
    }
</style>
