<script>
    import Step from "./Step.svelte";
    import picMidterms from '$lib/image/pic-midterms.png';

    let steps = [
        { name: 'DaveStore', icon: 'fa-solid fa-cart-shopping' },
        { name: 'Workshop', icon: 'fa-solid fa-list-check' },
        { name: 'Projects', icon: 'fa-solid fa-diagram-project' }
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <hr class="my-10 border-t-2 border-dark-green" />

    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="relative shadow-2xl grid place-items-center">
            <!-- Added border and padding for offset -->
            <img src={picMidterms} alt="" class="object-cover z-[2] max-h-[70vh] max-w-[70vh] rounded-full border-4 border-white p-2 shadow-lg" />
        </div>
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl text-white">
                Hi! I'm <span class="poppins text-dark-green">Dave Justin</span> Arcilla<br />Front End
                <span class="poppins text-dark-green">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl text-white">
                My <span class="text-dark-green">favorite tech</span> includes JavaScript (SvelteKit), TailwindCSS, CSS, and HTML.
            </p>
        </div>
    </section>     

    <hr class="my-10 border-t-2 border-dark-green" />
</main>

<style>
    /* Custom CSS for dark green color */
    .text-dark-green {
        color: #246624; /* Dark green color */
    }
</style>
