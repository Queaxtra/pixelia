<script>
    import Footer from "./Footer.svelte";
    import Navbar from "./Navbar.svelte";
    import News from "./News.svelte";
</script>

<header class="relative w-full h-80 md:h-[400px] lg:h-[400px] bg-cover -mt-10" style="background-image: url('https://cdn.discordapp.com/attachments/1136591322208272385/1186702678710046770/png-repeat.png?ex=659435fe&is=6581c0fe&hm=ce36e4ac8ae6aee34aebadfdd287d5acfd6d87652078047a05d1fe6cc677aa3d');">
    <div class="absolute right-0 top-0 invisible md:invisible lg:visible">
        <img class="w-full md:w-[30rem]" src="https://cdn.discordapp.com/attachments/1136591322208272385/1186703417419239496/hotelview.png?ex=659436ae&is=6581c1ae&hm=f9779b4d8e4a85bc0d700b2b4bbf387bde6eb56c59afca94c6ab70e5c2c6fc90&" alt="Hotel View">
    </div>
    
    <Navbar />

    <div class="m-5 md:m-10 lg:m-10 mx-2 md:mx-10 lg:mx-10">
        <h1 class="text-3xl md:text-4xl lg:text-4xl font-bold -mt-10 md:mt-0 lg:mt-0 mx-3 md:mx-0 lg:mx-0 transition-all duration-300">Pixels to Fun, Way to Go!</h1>
        <p class="text-sm md:text-base lg:text-base md:w-96 lg:w-96 my-2 md:my-5 lg:my-5 mx-3 md:mx-0 lg:mx-0 transition-all duration-300">We offer you much more than chatting and building, be a part of us and let us surprise you.</p>
        <div class="mt-3 mx-3 md:mx-0 lg:mx-0">
            <button class="text-xs md:text-base lg:text-base px-5 md:px-7 lg:px-7 py-2.5 bg-green-500 hover:bg-green-600 rounded-full transition-all duration-300"><i class="fa-solid fa-right-to-bracket"></i> Login Now</button>
            <button class="text-xs md:text-base lg:text-base px-5 md:px-7 lg:px-7 py-2.5 bg-blue-500 hover:bg-blue-600 rounded-full transition-all duration-300"><i class="fa-solid fa-unlock"></i> Register for Free</button>
        </div>
    </div>
    
    <News />
    <Footer />
</header>
