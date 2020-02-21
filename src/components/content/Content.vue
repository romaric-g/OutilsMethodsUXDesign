<template>
    <section>
        <div>
            <div class="big-title-box">
                <h1 class="big-title">{{ title }}</h1>
            </div>
            <div class="section-content" :class="{ reverse }">
                <div class="image-box">
                    <slot name="illu"></slot>
                </div>
                <div class="content-box">
                    <slot></slot>         
                </div>
            </div>
            <slot name="reminder"></slot>
        </div>
    </section>
</template>

<script>
import Items from "./elements/Items"
import Description from "./elements/Description"
import Reminder from "./elements/Reminder"
export default {
    components: {Items, Reminder, Description},
    props: ["title","reverse"]
}
</script>

<style lang="scss" scoped>
section {
    min-height: 100vh;
    max-width: 1100px;
    padding: 20px;
    width: 100%;
    margin: 0 auto;

    .big-title-box {
        margin: 20px 0;
        text-align: right;
        .big-title {
            font-family: "Montserrat", sans-serif;
            font-size: 2.6em;
            display: inline-block;
            position: relative;
            text-transform: uppercase;

            &:after {
                content: "";
                position: absolute;
                bottom: -2px;
                height: 2px;
                left: 0;right: 0;
                background-color: black;
            }
        }    
    }

    .section-content {
        display: flex;
        align-items: center;

        &.reverse {
            .image-box {
                order: 2;
            }
        }

        .image-box, .content-box {
            flex: 1;
            width: 50%;
        }

        .image-box {
            svg {
                width: 100%;
                transform: scale(0.9)
            }
        }

        .content-box {
            & > * {
                margin: 20px 0;
            }
        }
    }

    @media screen and (max-width: 1000px) {
        .section-content {
            flex-direction: column;

            .image-box, .content-box {
                width: 100%;
            }
        }

        .big-title-box .big-title {
            font-size: 2em;
        }
    }

    @media screen and (max-width: 600px) {
        .big-title-box .big-title {
            font-size: 1.8em;
        }
    }
}

</style>