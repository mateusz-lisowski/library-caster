<script lang="ts">
	import { AppBar, Avatar } from '@skeletonlabs/skeleton';
    import { popup } from '@skeletonlabs/skeleton';
    import type { PopupSettings } from '@skeletonlabs/skeleton';
	import AvatarPopup from './AvatarPopup.svelte';
    
    const popupFeatured: PopupSettings = {
        // Represents the type of event that opens/closed the popup
        event: 'click',
        // Matches the data-popup value on your popup element
        target: 'popupFeatured',
        // Defines which side of your trigger the popup will appear
        placement: 'bottom',
    };
					
</script>			

<AvatarPopup dataPopup="popupFeatured"/>

<AppBar>
    <svelte:fragment slot="lead">
        <div class="flex">
            <a href="/" class="btn-icon bg-initial">
                <img src="favicon.png" alt="Library caster's icon" />
            </a>
            <a href="/" class="btn bg-initial">
                <strong class="text-2xl">Library Caster</strong>
            </a>
        </div>
    </svelte:fragment>
    <svelte:fragment slot="trail">
        <a href="/" class="btn bg-initial font-semibold">Home</a>
        <a href="/pricing" class="btn bg-initial font-semibold">Pricing</a>
        <a href="/dashboard" class="btn bg-initial font-semibold">Dashboard</a>
        <button type="button" class="btn bg-initial" use:popup={popupFeatured}>
            <Avatar src="placeholder.jpeg" width="w-10" rounded="rounded-full" />
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
            </svg>              
        </button>
    </svelte:fragment>
</AppBar>