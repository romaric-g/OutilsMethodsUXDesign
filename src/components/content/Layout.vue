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
                    <p>Le focus group c’est : regrouper vos “cibles” pour leur poser des questions lors d’une séance de discussion. Elle est mené par un modérateur qui lance et structure les discussions, tout en leur donnant de la vie. Le but étant de recueillir la perception, les idées et envie des participants, pour que le contenu final réponde à leur besoin. Des idées auxquelles l’équipe n’aurait pas pensé à l’avance peuvent finir par être évoquées. Et oui, la discussion amène la créativité et la critique !</p>
                </Description>
                <Items title="Comment ?">
                    <p>Comme toute manifestation impliquant un groupe, il faut organiser l’événement des semaines à l’avance. Avant de se lancer, il faudra donc définir les objectifs de la recherche, établir des profils </p>
                    <p>ciblés, rechercher des participants et les recruter ( il peut y avoir besoin d’un questionnaire pour être sûr qu’ils répondent aux critères ), et bien entendu, il ne faut pas oublier de décider d’un modérateur.</p>
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