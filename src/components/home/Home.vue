<template>
    <header>
        <p>{{text}}</p>
        <button @click="change">Change</button>
    </header>
</template>

<script>
export default {
    data() {
        return {
            text: "Bienvenue sur la page d'accueil!"
        }
    },
    methods: {
        change() {
            this.text = this.text + "Romaric le dieux" + " ";
        }
    }
}
</script>

<style lang="scss">
p {
    a {

    }
}

</style>