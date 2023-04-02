<script setup>
    const props = defineProps({
        title: String,
        links: Object
    })
</script>

<template>
    <div class="w-full bg-slate-900 flex gap-1 p-3 items-center">
        <h1 class="text-4xl text-white">{{title}}</h1>
        <div class="flex flex-grow-1 mr-auto items-center">
            <a  v-for="link in links" :key="link.id" :href="link.url" class="text-white">
                {{ link.text }}
            </a>
        </div>
        <div>
            <h1 >test</h1>
        </div>
    </div>
</template>