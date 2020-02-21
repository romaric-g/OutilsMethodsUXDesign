<template>
    <section :id="ink" :class="colors">
        <div>
            <div class="big-title-box">
                <h1 class="big-title">{{ title }}</h1>
            </div>
            <div class="section-content" :class="{ reverse }">
                <div v-if="!noimage" class="image-box">
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
    props: ["title","reverse","ink","noimage","color"],
    data() {
        return {
            colorID: this.$props.color || 0
        }
    },
    computed: {
            colors: function() {
                return {
                    yellow: this.colorID == 1,
                    blue: this.colorID == 2,
                    red: this.colorID == 3,
                    green: this.colorID == 4,
                }
            }
    },
}
</script>

<style lang="scss" scoped>
section {
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

section.yellow {
    .big-title:after {
        background-color: var(--section-color-yellow);
    }
}
section.blue {
    .big-title:after {
        background-color: var(--section-color-blue);
    }
}
section.red {
    .big-title:after {
        background-color: var(--section-color-red);
    }
}
section.green {
    .big-title:after {
        background-color: var(--section-color-green);
    }
}

</style>