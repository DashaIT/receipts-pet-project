<script setup lang="ts">
const props = withDefaults(defineProps<{
    variant: 'primary' | 'secondary'
}>(), {
    variant: 'primary'
})

</script>

<template>
    <button class="button" :class="props.variant">
        <slot/>
    </button>
</template>

<style lang="scss" src="./VButton.scss"></style>