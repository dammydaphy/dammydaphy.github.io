<script>
    import Step from "./Step.svelte";
    import picMidterms from '$lib/image/pic-midterms.png';
    import gcccsaco from '$lib/image/gcccsaco.png';

    let steps = [
        { name: 'DaveStore', icon: 'fa-solid fa-cart-shopping' },
        { name: 'Workshop', icon: 'fa-solid fa-list-check' },
        { name: 'Projects', icon: 'fa-solid fa-diagram-project' }
    ];
</script>
<br><br><br><br><br><br>

<div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg-gap-10">
    <Step step={{ name: 'Weather App', icon: 'fa-solid fa-sun' }}>
        <a href="https://github.com/karomips/weather-app2" target="_blank" class="block p-4 bg-white rounded-lg transition-transform transform hover:scale-105 shadow-lg">
            
            <p class="text-black">The Weather App provides real-time weather updates <strong class="text-dark-green">using a weather API</strong>. Thank you!</p>
        </a>
    </Step>
    <Step step={{ name: 'Push Notification App', icon: 'fa-solid fa-bell' }}>
        <a href="https://github.com/Dumgrammer/pushnotiftracer" target="_blank" class="block p-4 bg-white rounded-lg transition-transform transform hover:scale-105 shadow-lg">
            <img src={gcccsaco} alt="" class="object-cover z-[2] max-h-[70vh] max-w-[37vh] rounded-full border-4 border-white p-2 shadow-lg" />
                <br><br><br><br>
            <p class="text-black">The Push Notification App allows users to receive alerts <strong class="text-dark-green">for important events and updates</strong>. Thank you!</p>
        </a>
    </Step>
    <Step step={{ name: 'Task Tracker', icon: 'fa-solid fa-tasks' }}>
        <a href="https://github.com/PickleC137/TaskTraker" target="_blank" class="block p-4 bg-white rounded-lg transition-transform transform hover:scale-105 shadow-lg">
            <p class="text-black">The Task Tracker helps users manage their tasks <strong class="text-dark-green">effectively and efficiently</strong>. Thank you!</p>
        </a>
    </Step>
</div>      