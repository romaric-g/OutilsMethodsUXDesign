<template>
    <main>
        <div class="menu">
            <Menu />
        </div>
        <div class="content">
            <Content title="Entretiens">
                <Description>
                    <h2>Mener un entretien</h2>
                    <p>Pour comprendre les besoins de vos utilisateurs, la méthode la plus simple est d’interroger directement de potentiels utilisateurs de votre service, ils seront plus apte à savoir ce qu’ils souhaitent que vous sur le sujet.</p>
                </Description>
                <Items title="Le principe est simple">
                    <p>En amont de l’entretien, préparez des questions. Veillez à ce qu’elles soient suffisamment ouverte, pour obtenir un grand nombre d’informations ( un simple oui ou non n’est pas très constructif )</p>
                    <p>Questionnez, prenez des notes, enregistrez les entretiens, de quoi se rappeler de ce qui à été dit </p>
                </Items>
                <template v-slot:reminder>
                   <Reminder /> 
                </template>
            </Content>
            <Content title="Autre titre" reverse="true">
                <Description>
                    <h2>Mener un entretien</h2>
                    <p>Pour comprendre les besoins de vos utilisateurs, la méthode la plus simple est d’interroger directement de potentiels utilisateurs de votre service, ils seront plus apte à savoir ce qu’ils souhaitent que vous sur le sujet.</p>
                </Description>
                <Items title="Le principe est simple">
                    <p>En amont de l’entretien, préparez des questions. Veillez à ce qu’elles soient suffisamment ouverte, pour obtenir un grand nombre d’informations ( un simple oui ou non n’est pas très constructif )</p>
                    <p>Questionnez, prenez des notes, enregistrez les entretiens, de quoi se rappeler de ce qui à été dit </p>
                </Items>
                <template v-slot:reminder>
                   <Reminder /> 
                </template>
            </Content>
            <Content title="BrainStorming">
                <Description>
                    <h2>Mener un entretien</h2>
                    <p>Pour comprendre les besoins de vos utilisateurs, la méthode la plus simple est d’interroger directement de potentiels utilisateurs de votre service, ils seront plus apte à savoir ce qu’ils souhaitent que vous sur le sujet.</p>
                </Description>
                <Items title="Le principe est simple">
                    <p>En amont de l’entretien, préparez des questions. Veillez à ce qu’elles soient suffisamment ouverte, pour obtenir un grand nombre d’informations ( un simple oui ou non n’est pas très constructif )</p>
                    <p>Questionnez, prenez des notes, enregistrez les entretiens, de quoi se rappeler de ce qui à été dit </p>
                </Items>
                <template v-slot:reminder>
                   <Reminder /> 
                </template>
            </Content>
        </div>
    </main>
</template>

<script>
import Content from "./Content";
import Menu from "./../menu/Menu";

import Items from "./elements/Items"
import Description from "./elements/Description"
import Reminder from "./elements/Reminder"

export default {
    name: "layout",
    components: {Menu, Content, Items, Description, Reminder}
}
</script>

<style lang="scss">
main {
    display: grid;
    grid-template-columns: auto 1fr;
    position: sticky;

    & > .menu {
        position: sticky;
        top: 0;
        height: 100vh;
    }
}
</style>