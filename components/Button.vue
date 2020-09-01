<template>
    <a :href="href" class="">
        <slot></slot>
    </a>
</template>

<script>
export default {
    props: [
        'type',
        'href',
    ]
}
</script>
