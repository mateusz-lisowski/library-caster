<script>
	import PriceCard from "$lib/components/PriceCard.svelte";
</script>

<div class="h-screen">
    <div class="flex flex-col items-center m-16 gap-4">
        <h2 class="h2">Pricing</h2>
        <span>Check our pricing plans and choose most suited for your needs.</span>
    </div>
    <div class="flex justify-around m-16">
        <PriceCard 
            planName="Basic" 
            planDescription="Free usage for up to 3 libaries. Every other plan incluedes the free plan also."
            benefits={[
                "Free up to 3 libraies", 
                "Community support", 
                "Adding books from admin dashboard"
                ]}
        />
        <PriceCard 
            planName="Pro" 
            planDescription="Plan for commertial usage. Most suitable for small buisness and idividuals working with libararies proffesionally."
            benefits={[
                "All benefits from Basic plan", 
                "Unlimited books in each libary", 
                "Up to 9 additional libaries", 
                "Possibility of adding books form mobile app level"
                ]}
        />
        <PriceCard 
            planName="Professional" 
            planDescription="Professional plan for enerprises. Custom assistance and 24/7 awarness. Contatct us to learn more."
            benefits={[
                "All benefits from Pro plan", 
                "Unlimited books in library", 
                "Unlimited libaries", 
                "Dedicated support", 
                ]}
        />

    </div>
</div>