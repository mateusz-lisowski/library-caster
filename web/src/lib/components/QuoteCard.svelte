<script lang="ts">
    export let content: string;
    export let author: string;
</script>

<div class="card card-hover flex flex-col justify-between p-4">
    <blockquote class="blockquote">{content}</blockquote>
    <div class="h-4"></div>
    <strong>{author}</strong>
</div>