<template>
    <nav :class="{open}">
        <div class="head">
            <p class="reduce">Réduire le menu</p>
        </div>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            open: true
        }
    }
}
</script>

<style lang="scss">
nav {
    width: 400px;
    height: 100vh;
}
</style>