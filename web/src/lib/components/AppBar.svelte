<script lang="ts">
	import { AppBar } from '@skeletonlabs/skeleton';
</script>


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
        <a
            class="btn btn-sm variant-ghost-surface"
            href="https://discord.gg/EXqV7W8MtY"
            target="_blank"
            rel="noreferrer"
        > 
            Discord
        </a>
        <a
            class="btn btn-sm variant-ghost-surface"
            href="https://twitter.com/SkeletonUI"
            target="_blank"
            rel="noreferrer"
        >
            Twitter
        </a>
        <a
            class="btn btn-sm variant-ghost-surface"
            href="https://github.com/skeletonlabs/skeleton"
            target="_blank"
            rel="noreferrer"
        >
            GitHub
        </a>
    </svelte:fragment>
</AppBar>