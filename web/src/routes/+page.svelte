<script>
    import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
    import QuoteCard from '$lib/components/QuoteCard.svelte';
</script>


<div class="flex justify-center items-center h-screen gap-8 m-16">
    <div class="flex flex-col gap-8 w-1/2">
        <div class="ml-8"><img class="w-24" src="favicon.png" alt="Library caster's icon" /></div>
        <h1 class="h1 text-6xl">Library Caster</h1>
        <span class="text-2xl">Manage your library like never before! Never forget your best memories with books thnaks to this innovative library managment service.</span>
        <div class="flex gap-8 m-4">
            <button type="button" class="btn variant-filled-primary">
                <span>Check more</span>
                <span>
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
                    </svg>
                </span>
            </button>
            <button type="button" class="btn variant-filled">
                <span>Get started</span>
                <span>
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 6H5.25A2.25 2.25 0 0 0 3 8.25v10.5A2.25 2.25 0 0 0 5.25 21h10.5A2.25 2.25 0 0 0 18 18.75V10.5m-10.5 6L21 3m0 0h-5.25M21 3v5.25" />
                    </svg>              
                </span>
            </button>
        </div>
    </div>
    <img class="w-1/2 rounded-md" src="placeholder.jpeg" alt="Placeholder">
</div>

<div class="m-16">
    <h2 class="h2">We have been trusted by many clients.</h2>
    <div class="grid grid-cols-3 gap-8 m-8">
        <QuoteCard 
            content="Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                Nihil porro ducimus, quia alias, sit labore sed possimus velit natus incidunt officia voluptatibus dolore. " 
            author="CEO of the Longscope™ Inc." 
        />
        <QuoteCard 
            content="Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                Nihil porro ducimus, quia alias, sit labore sed possimus velit natus incidunt officia voluptatibus dolore. 
                Praesentium, facilis nulla? Ipsam quos modi voluptatem" 
            author="CEO of the Longscope™ Inc." 
        />
        <QuoteCard content="Lorem ipsum dolor sit, amet consectetur adipisicing elit. " author="CEO of the Longscope™ Inc." />
        <QuoteCard 
            content="Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                Nihil porro ducimus, quia alias, sit labore sed possimus velit natus incidunt officia voluptatibus dolore. " 
            author="CEO of the Longscope™ Inc." 
        />
    </div>
</div>

<div class="m-16">
    <div class="card flex flex-col gap-4 p-4 text-xl">
        <h2 class="h2 text-2xl">Here are all most frequently asked questions</h2>
        <hr />
        <Accordion>
            <AccordionItem open>
                <svelte:fragment slot="lead">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v12m-3-2.818.879.659c1.171.879 3.07.879 4.242 0 1.172-.879 1.172-2.303 0-3.182C13.536 12.219 12.768 12 12 12c-.725 0-1.45-.22-2.003-.659-1.106-.879-1.106-2.303 0-3.182s2.9-.879 4.006 0l.415.33M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                    </svg>                      
                </svelte:fragment>
                <svelte:fragment slot="summary">Is the serveice free?</svelte:fragment>
                <svelte:fragment slot="content">
                    Yes, our service is completly free for basic usage for everone. 
                    If you want to upgarade to the next level, feel free to contact our sales department.
                </svelte:fragment>
            </AccordionItem>
            <AccordionItem>
                <svelte:fragment slot="lead">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="m15.75 15.75-2.489-2.489m0 0a3.375 3.375 0 1 0-4.773-4.773 3.375 3.375 0 0 0 4.774 4.774ZM21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                    </svg>                  
                </svelte:fragment>
                <svelte:fragment slot="summary">How much libraries can I mange for free?</svelte:fragment>
                <svelte:fragment slot="content">You can manage up to 3 libraries without any need to pay 😄.</svelte:fragment>
            </AccordionItem>
            <AccordionItem>
                <svelte:fragment slot="lead">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M12 9v6m3-3H9m12 0a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                    </svg>                                   
                </svelte:fragment>
                <svelte:fragment slot="summary">How to add new books to my libary?</svelte:fragment>
                <svelte:fragment slot="content">
                    To add new books to your library you have 2 options. 
                    Either you can add them from the admin dashboard in the browser, or scan them from your smartphone app.
                </svelte:fragment>
            </AccordionItem>
        </Accordion>
    </div>
    
</div>
