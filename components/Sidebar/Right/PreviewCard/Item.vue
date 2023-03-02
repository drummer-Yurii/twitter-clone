<template>
    <div class="p-3 border-b hover:bg-gray-100 cursor-pointer dark:hover:bg-dim-300" :class="wrapperClasses">
        <slot></slot>
    </div>
</template>

<script setup>
const { defaultTransition, twitterBorderCollor } = useTailwindConfig();
const wrapperClasses = computed(() => `${defaultTransition} ${twitterBorderCollor}`)
</script>