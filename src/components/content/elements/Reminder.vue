<template>
    <div class="reminder">
                <h2 class="r-title">{{ title }}</h2>
                <div class="reminder-content">
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
    .reminder {
        background-color: #3F3D56;
        font-family: "Montserrat", sans-serif;
        font-size: 1em;
        padding: 10px 20px;
        margin: 40px 0;
        text-align: left;

        .r-title {
            color: white;
            text-align: center;
            font-weight: 700;
            font-size: 1.2em;
            padding: 10px 0;
        }

        .reminder-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-auto-rows: 1fr;
            grid-row-gap: 1rem;
            grid-column-gap: 1rem;
            font-weight: 400;
            padding: 10px;

            .inter-box {
                display: flex;
                align-items: center;

                p {
                    margin: 0 20px;
                    color: white;
                }
            }
        }
        @media screen and (max-width: 800px) { 
            .reminder-content { 
                grid-template-columns: 1fr;
            }
        }
    }
</style>