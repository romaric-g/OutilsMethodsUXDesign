<template>
    <div class="items-box">
        <h3>{{title}}</h3>
        <div class="content">
            <slot></slot>
        </div>
    </div>   
</template>

<script>
export default {
    props: ["title"]
}
</script>

<style lang="scss">
    .items-box {
        .content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-column-gap: 1rem;
        }
        @media screen and (max-width: 800px) { 
            .content {
                grid-template-columns: 1fr;
                grid-row-gap: 1rem;
            }
        }
    }
</style>