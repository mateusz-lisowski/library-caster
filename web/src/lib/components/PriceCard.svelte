<script lang="ts">
    export let planName: string;
    export let planDescription: string;
    export let benefits: string[];
</script>

<div class="card card-hover w-96 flex flex-col justify-between p-8 gap-8 items-center border-2 border-surface-500">
            
    <h3 class="h3">{planName}</h3>
    <span>{planDescription}</span>
    
    <hr class="w-full"/>

    <ul class="list w-full flex flex-col gap-4">
        {#each benefits as benefit}
            <li>
                <span>
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                    </svg>                          
                </span>
                <span class="flex-auto font-semibold">{benefit}</span>
            </li>
        {/each}
    </ul>
    
    <hr class="w-full"/>

    <button type="button" class="btn variant-filled-primary w-full">
        <span>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25 21 12m0 0-3.75 3.75M21 12H3" />
            </svg>                      
        </span>
        <span>Check out {planName} plan</span>
    </button>
</div>