<template>
    <a :href="link"><slot></slot></a>
</template>

<script>
export default {
    props: ['link']
}
</script>

<style lang="scss" scoped>
    a {
        display: block;
        width: 48px;
        height: 48px;
    }
</style>