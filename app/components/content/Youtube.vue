<script setup lang="ts">
defineProps<{ videoid: string }>();
</script>

<template>
    <div class="not-prose mx-auto max-w-3xl w-full aspect-video overflow-hidden rounded-lg">
        <ClientOnly>
            <iframe
                :src="`https://www.youtube.com/embed/${videoid}`"
                class="h-full w-full"
                frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen
            />
        </ClientOnly>
    </div>
</template>
