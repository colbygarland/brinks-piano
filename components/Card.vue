<template>
    <div class="max-w-sm rounded overflow-hidden shadow-lg">
        <img class="w-full h-48 object-cover" :src="image" :alt="title">
        <div class="px-6 py-4">
            <div class="font-bold text-xl mb-2">{{ title }}</div>
            <p class="text-gray-700 text-base">
            {{ desc }}
            </p>
        </div>
    </div>
</template>

<script>
    export default {
        props: [
            'image',
            'alt',
            'title', 
            'desc',
        ]
    }
</script>