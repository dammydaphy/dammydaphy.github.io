<script>
    export let y;

    let tabs = [
        { name: "Projects", link: "/projects" },
        { name: "About me", link: "/about" }
        // {name: "Blog", link:"#blog"}, 
    ];
</script>

<header class={'sticky z-[10] top-0 duration-200 w-full flex items-center justify-between border border-solid ' + (
    y > 0 
    ? "py-4 bg-slate-950 border-violet-950"
    : "py-6 bg-transparent border-transparent"
) + ' text-white'}>
    <h1 class="font-medium text-2xl sm:text-3xl">
        <b class="fold-bold poppins">ITE 316</b> Midterm Project
    </h1>
    
    <!-- Combined Tabs and Button in a Flex Container -->
    <div class="flex items-center gap-6">
        <div class="flex gap-6">
            {#each tabs as tab}
                <a href={tab.link} class="text-lg duration-200 hover:text-violet-400 transition-colors shadow-md p-1 rounded-md">
                    <p class="shadow-sm">{tab.name}</p>
                </a>
            {/each}
        </div>
        
        <!-- New Button to Navigate to Homepage -->
        <a 
            href="https://dammydaphy.github.io"
            class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-violet-500 text-white shadow-lg transition-transform transform hover:scale-105">
            <div class="absolute top-0 right-full w-full h-full bg-violet-700 opacity-20 group-hover:translate-x-full z-0 duration-200"></div>
            <h4 class="relative z-10">Home</h4>
        </a>

        <a 
            href="https://www.facebook.com/djra.25/"
            target="_blank"
            class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950 shadow-lg transition-transform transform hover:scale-105">
            <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"></div>
            <h4 class="relative z-10">Message me</h4>
        </a>
    </div>
</header>
