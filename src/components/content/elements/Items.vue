<template>
    <div class="items-box">
        <h3> Le principe est simple</h3>
        <div class="content">
            <div class="item">
                <p> En amont de l’entretien, préparez des questions. Veillez à ce qu’elles soient suffisamment ouverte, pour obtenir un grand nombre d’informations ( un simple oui ou non n’est pas très constructif )</p>
            </div>
            <div class="item">
                <p>Questionnez, prenez des notes, enregistrez les entretiens, de quoi se rappeler de ce qui à été dit </p>
            </div>
        </div>
    </div>   
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
    .items-box {
        .content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-column-gap: 1rem;
        }
    }
</style>