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
                   <Reminder title="Mener vos entretiens à la perfection">
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="30.849" height="30.849" viewBox="0 0 30.849 30.849"><path id="Icon_metro-warning" data-name="Icon metro-warning" d="M17.995,4.723,30.922,30.487H5.068L17.995,4.723Zm0-2.795a2.23,2.23,0,0,0-1.834,1.345L2.994,29.516c-1.009,1.793-.151,3.261,1.907,3.261H31.089c2.058,0,2.916-1.467,1.907-3.261h0L19.829,3.273a2.23,2.23,0,0,0-1.834-1.345Zm1.928,25.064a1.928,1.928,0,1,1-1.928-1.928A1.928,1.928,0,0,1,19.923,26.992Zm-1.928-3.856a1.928,1.928,0,0,1-1.928-1.928V15.424a1.928,1.928,0,1,1,3.856,0v5.784A1.928,1.928,0,0,1,17.995,23.136Z" transform="translate(-2.571 -1.928)" fill="#fff"/></svg>
                            <p>Informez le participant de la raison de l’entretien avant de le commencer</p>
                        </div>
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="33" viewBox="0 0 24 33"><path id="Icon_material-loop" data-name="Icon material-loop" d="M18,6V1.5l-6,6,6,6V9a9.007,9.007,0,0,1,9,9,8.806,8.806,0,0,1-1.05,4.2l2.19,2.19A11.979,11.979,0,0,0,18,6Zm0,21a9.007,9.007,0,0,1-9-9,8.806,8.806,0,0,1,1.05-4.2L7.86,11.61A11.979,11.979,0,0,0,18,30v4.5l6-6-6-6Z" transform="translate(-6 -1.5)" fill="#fff"/></svg>
                            <p>Laissez le parler !</p>
                        </div>
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="33" height="33" viewBox="0 0 33 33"><g id="Icon_feather-info" data-name="Icon feather-info" transform="translate(-1.5 -1.5)"><path id="Tracé_173" data-name="Tracé 173" d="M33,18A15,15,0,1,1,18,3,15,15,0,0,1,33,18Z" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/><path id="Tracé_174" data-name="Tracé 174" d="M18,24V18" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/><path id="Tracé_175" data-name="Tracé 175" d="M18,12h0" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/></g></svg>
                            <p>Ne l’influencez pas pour qu’il réponde à vos attentes personnelles.</p>
                        </div>

                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 30 30"><path id="Icon_feather-message-circle" data-name="Icon feather-message-circle" d="M31.5,17.25a12.57,12.57,0,0,1-1.35,5.7A12.75,12.75,0,0,1,18.75,30a12.57,12.57,0,0,1-5.7-1.35L4.5,31.5l2.85-8.55A12.57,12.57,0,0,1,6,17.25a12.75,12.75,0,0,1,7.05-11.4,12.57,12.57,0,0,1,5.7-1.35h.75a12.72,12.72,0,0,1,12,12Z" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/></svg>
                            <p>Réaliser une dizaine d'entretiens.</p>
                        </div>
                    </Reminder> 
                </template>
            </Content>
            <Content title="FOCUS GROUP" reverse="true">
                <Description>
                    <p>Le focus group c’est : regrouper vos “cibles” pour leur poser des questions lors d’une séance de discussion. Elle est mené par un modérateur qui lance et structure les discussions, tout en leur donnant de la vie. Le but étant de recueillir la perception, les idées et envie des participants, pour que le contenu final réponde à leur besoin. Des idées auxquelles l’équipe n’aurait pas pensé à l’avance peuvent finir par être évoquées. Et oui, la discussion amène la créativité et la critique !</p>
                </Description>
                <Items title="Comment ?">
                    <p>Comme toute manifestation impliquant un groupe, il faut organiser l’événement des semaines à l’avance. Avant de se lancer, il faudra donc définir les objectifs de la recherche, établir des profils </p>
                    <p>ciblés, rechercher des participants et les recruter ( il peut y avoir besoin d’un questionnaire pour être sûr qu’ils répondent aux critères ), et bien entendu, il ne faut pas oublier de décider d’un modérateur.</p>
                </Items>
                <template v-slot:reminder>
                   <Reminder title="Le jour de la rencontre">
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="33" height="33" viewBox="0 0 33 33">
                            <g id="Icon_feather-clock" data-name="Icon feather-clock" transform="translate(-1.5 -1.5)">
                                <path id="Tracé_337" data-name="Tracé 337" d="M33,18A15,15,0,1,1,18,3,15,15,0,0,1,33,18Z" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                <path id="Tracé_338" data-name="Tracé 338" d="M18,9v9l6,3" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                            </g>
                            </svg>
                            <p>15 min de briefing de départ</p>
                        </div>
                        
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="33" height="33" viewBox="0 0 33 33">
                            <g id="Icon_feather-clock" data-name="Icon feather-clock" transform="translate(-1.5 -1.5)">
                                <path id="Tracé_337" data-name="Tracé 337" d="M33,18A15,15,0,1,1,18,3,15,15,0,0,1,33,18Z" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                <path id="Tracé_338" data-name="Tracé 338" d="M18,9v9l6,3" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                            </g>
                            </svg>
                            <p>15 min de débriefing</p>
                        </div>
                        <div class="inter-box">
                            <p>Entre 1h et 2h de discussion</p>
                        </div>
                    </Reminder> 
                </template>
            </Content>
            <Content title="OBSERVATION">
                <Description>
                    <h2>Mener un entretien</h2>
                    <p>Cela consiste à aller sur le terrain afin de recueillir des données sur une population ou un groupe d’individus. Les données sont simplement récoltées par observation, comme il est dit dans le nom de la méthode. Ce qu’il est important de retenir est qu’il ne faut jamais influencer sur les résultats, il s’agit juste d’une observation. </p>
                </Description>
                <Items title="Comment ?">
                    <p>Avant de mener une observation, il vous faut définir les paramètres et les contextes d’observations: Quels sont les éléments qu’il serait intéressant d’observer et quand et où doit on allez faire ces observations.</p>
                </Items>
                <template v-slot:reminder>
                   <Reminder title="Les avantages">
                        <div class="inter-box">
                            <p>Récupérer des données par l’observation permet de faire émerger le non-verbal et des problématiques insoupçonnées auxquelles doit faire face la cible potentielle dans son environnement naturel.</p>
                        </div>
                        <div class="inter-box">
                            <p>vous répondrez pleinement aux besoins de la cible, et pourrez d’ailleurs surement toucher un plus grand public.</p>
                        </div>
                    </Reminder> 
                </template>
            </Content>
            <Content title="PERSONA" reverse="true">
                                <Description>
                                    <h2>La méthode des personas</h2>
                                    <p>La méthode des personas aide l’équipe à changer de perspective et à rester focalisé sur les utilisateurs cible afin de mieux répondre à leurs besoins et de créer une expérience positive et engageante. Un Persona est une personnalité fictive qui décrit la plupart du temps un prospect type. </p>
                                </Description>
                                <Items title="Créer un persona">
                                    <p>Pour créer un persona, il est nécessaire de réaliser des enquêtes auprès de vos cibles afin de mieux les connaîtres. Une fois un grand nombre d’enquête effectué, vous allez pouvoir dresser un ou plusieurs Persona “type”. Ils permettent de mieux définir les stratégies à appliquer dans le développement d’un projet tier.</p>
                                </Items>
                                <template v-slot:reminder>
                                <Reminder title="Pourquoi cette méthode ? ">
                                        <div class="inter-box"> 
                                            <p>«En donnant vie à nos utilisateurs cible, on donne vie à notre projet : et tant il y a de la vie, il y a de l’espoir ! » </p>
                                        </div>
                                    </Reminder> 
                                </template>
            </Content>
            <Content title="EXPERIENCE MAP">
                <Description>
                    <h2>Mener un entretien</h2>
                    <p>L’expérience map c’est créer la “cartographie” de l’expérience utilisateur. Il s’agit d’analyser toutes les étapes par lesquelles passe l’utilisateur lors de son expérience : pensées, actions, émotions. Vous connaîtrez ainsi son cheminement complet vers la réalisation d’une tâche similaire à celle que vous allez concevoir. C’est cette cartographie qui donne vie au persona. Vous pourrez ainsi créer un produit qui lui procurera une meilleure expérience utilisateur.  </p>
                </Description>
                <template v-slot:reminder>
                   <Reminder title="Ne vous inquiétez pas">
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="33" height="33" viewBox="0 0 33 33">
                                    <g id="Icon_feather-info" data-name="Icon feather-info" transform="translate(1.5 1.5)">
                                        <path id="Tracé_173" data-name="Tracé 173" d="M33,18A15,15,0,1,1,18,3,15,15,0,0,1,33,18Z" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                        <path id="Tracé_174" data-name="Tracé 174" d="M18,24V18" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                        <path id="Tracé_175" data-name="Tracé 175" d="M18,12h0" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                    </g>
                            </svg>  
                            <p>Mais ne vous inquiétez pas, il est normal que cette cartographie change avec le temps, vous découvrirez toujours de nouveaux problèmes et de nouvelles solutions ! </p>
                        </div>
                    </Reminder> 
                </template>
            </Content>
            <Content title="COMPLÉTION DES PHRASES" reverse="true">
                <Description>
                    <h2>Complétion des phrases</h2>
                    <p>Le plus simple pour décrire cette méthode est de vous donner un exemple, il faut créer des phrases de ce genre : “Quand j’utilise ce produit, je me sens …” , à donner à l’utilisateur afin qu’il les complète. Cela permet d’évaluer de manière qualitative l’expérience de l’utilisateur grâce à leur feedback. </p>
                </Description>
                <Items title="Comment ?">
                    <p>Créez des phrases qui permettent de guider l’utilisateur vers le sujet que vous souhaitez aborder Donnez ensuite ces phrases dans un questionnaire aux utilisateurs afin qu’ils expriment leur ressenti sur le produit</p>
                </Items>
                <template v-slot:reminder>
                   <Reminder title="Pourquoi cette méthode ? ">
                        <div class="inter-box"> 
                            <p>Préparation très rapide</p>
                        </div>
                        <div class="inter-box"> 
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="33" viewBox="0 0 24 33">
                                <path id="Icon_material-loop" data-name="Icon material-loop" d="M18,6V1.5l-6,6,6,6V9a9.007,9.007,0,0,1,9,9,8.806,8.806,0,0,1-1.05,4.2l2.19,2.19A11.979,11.979,0,0,0,18,6Zm0,21a9.007,9.007,0,0,1-9-9,8.806,8.806,0,0,1,1.05-4.2L7.86,11.61A11.979,11.979,0,0,0,18,30v4.5l6-6-6-6Z" transform="translate(-6 -1.5)" fill="#fff"/>
                        </svg>
                            <p>Méthode flexible, s’utilise tout le long du projet</p>
                        </div>
                        <div class="inter-box"> 
                            <p>Permet d’avoir une bonne base de travail</p>
                        </div>
                    </Reminder> 
                </template>
            </Content>
            <Content title="BRAINSTORMING" reverse="true">
                <Description>
                    <p>Le plus simple pour décrire cette méthode est de vous donner un exemple, il faut créer des phrases de ce genre : “Quand j’utilise ce produit, je me sens …” , à donner à l’utilisateur afin qu’il les complète. Cela permet d’évaluer de manière qualitative l’expérience de l’utilisateur grâce à leur feedback. </p>
                </Description>
                <Items title="Voici les clés d’un brainstorming réussi et efficace:">
                    <p>Effectuez un brief, énoncez le sujet du brainstorming avec une thématique ou une problématique, l’écrire sur un tableau est conseillé.</p>
                    <p>Demandez à chaque participant d’écrire leurs idées sur des post it, à chaque idée un post it. Rassemblez les ensuites par grandes thématiques et affichez les sur un seul mur. </p>
                </Items>
                <template v-slot:reminder>
                   <Reminder title="Ne pas oublier le CQFD ">
                        <div class="inter-box"> 
                            <p>C, pour critique Abolie : aucune critique n’est autorisée.</p>
                        </div>
                        <div class="inter-box"> 
                            <p>Q,  pour quantité : plus il y a d’idée et mieux c’est</p>
                        </div>
                        <div class="inter-box"> 
                            <p>F, pour farfelue : être créatif et original</p>
                        </div>
                        <div class="inter-box"> 
                            <p>D, pour démultiplication : une idée en entraîne une autre.</p>
                        </div>
                    </Reminder> 
                </template>
            </Content>
            <Content title="STORYBOARD">
                <Description>
                    <h2>Qu’est ce que c’est ?</h2>
                    <p>Un storyboard est une BD très courte de 5 à 10 planches qui est dessiné par l’UX designer. Le but du storyboard est de montrer l’expérience et de raconter une histoire sur le produit à concevoir. Il permet de ne pas quitter l’objectif principal tout au long du projet et de se remettre sur les rails lorsque l’on perd de vue cet objectif. </p>
                </Description>
                <Items title="Créer un storyboard">
                    <p>Afin de créer un storyboard, il faut se baser sur les données recueillis lors de la phase de recherche Il doit impérativement être dessiné à l’aide d’un feutre noir (afin de ne pas trop rentrer dans les détails) Astuce: si vous ne savez pas dessiner, vous pouvez mettre des légendes/vignettes/indices temporels, vous pouvez aussi nommer les personnages ( on répète, tant qu’il y a de la vie, il y a de l’espoir ! ).</p>
                </Items>
                <template v-slot:reminder>
                   <Reminder title="Réussir un story board">
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="33" height="33" viewBox="0 0 33 33">
                                <g id="Icon_feather-info" data-name="Icon feather-info" transform="translate(1.5 1.5)">
                                    <path id="Tracé_173" data-name="Tracé 173" d="M33,18A15,15,0,1,1,18,3,15,15,0,0,1,33,18Z" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                    <path id="Tracé_174" data-name="Tracé 174" d="M18,24V18" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                    <path id="Tracé_175" data-name="Tracé 175" d="M18,12h0" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                </g>
                            </svg>
                            <p>le story board n’est pas un Wireframe et ne sert pas non plus à présenter le produit.</p>
                        </div>
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="30.857" height="27.416" viewBox="0 0 30.857 27.416">
                                <path id="Icon_metro-bubbles" data-name="Icon metro-bubbles" d="M31.714,29.281a3.128,3.128,0,0,0,1.714,2.791V32.5a6.377,6.377,0,0,1-5.5-1.93,8.612,8.612,0,0,1-2.217.288C21.454,30.857,18,27.787,18,24s3.454-6.857,7.714-6.857,7.714,3.07,7.714,6.857A6.325,6.325,0,0,1,32,27.977a3.111,3.111,0,0,0-.285,1.3ZM16.286,5.143C23.744,5.143,29.812,9.981,30,16a10.511,10.511,0,0,0-4.281-.9,10.208,10.208,0,0,0-6.807,2.523A8.462,8.462,0,0,0,15.964,24a8.219,8.219,0,0,0,.743,3.423c-.14,0-.28.006-.421.006a16.938,16.938,0,0,1-2.138-.135c-2.946,2.946-6.462,3.474-9.862,3.552v-.721c1.836-.9,3.429-2.538,3.429-4.41a5.173,5.173,0,0,0-.058-.769,10.49,10.49,0,0,1-5.085-8.66c0-6.154,6.14-11.143,13.714-11.143Z" transform="translate(-2.571 -5.143)" fill="#fff"/>
                            </svg>
                            <p>COMMUNICATION avec les autres membre du projet, c’est essentiel</p>
                        </div>
                    </Reminder> 
                </template>
            </Content>
            <Content title="TRI DE CARTE" reverse="true">
                <Description>
                    <h2>Qu’est ce que c’est ?</h2>
                    <p>Un animateur définit les cartes puis des utilisateurs les regroupent et nomment les catégories qu’ils ont créés. Cela permet, après analyse des résultats de créer une architecture du site autour de l’utilisateur.  </p>
                </Description>
                <Items title="Mise en oeuvre">
                    <p>Il faut commencer par écrire les cartes par rapport au contenu du site. Les cartes doivent décrire le contenu avec un titre (un ou deux mots) et une phrase descriptive. Chaque carte représente une fonctionnalité du site.</br>Donnez les cartes à un individu ou à un groupe d’individu afin qu’ils les catégorisent.  </p>
                </Items>
                <template v-slot:reminder>
                   <Reminder title="Pourquoi cette méthode ? ">
                        <div class="inter-box"> 
                            <svg xmlns="http://www.w3.org/2000/svg" width="33" height="33" viewBox="0 0 33 33">
                                <g id="Icon_feather-info" data-name="Icon feather-info" transform="translate(1.5 1.5)">
                                    <path id="Tracé_173" data-name="Tracé 173" d="M33,18A15,15,0,1,1,18,3,15,15,0,0,1,33,18Z" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                    <path id="Tracé_174" data-name="Tracé 174" d="M18,24V18" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                    <path id="Tracé_175" data-name="Tracé 175" d="M18,12h0" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                </g>
                            </svg>
                            <p>C’est un incontournable pour l’architecture d’informations Les participants se sentiront très concernés par le tri de carteLe traitement des résultats peut être facilité par de nombreux sites en ligneIl est recommandé de ne pas dépasser 50 cartes afin de ne pas perdre l’utilisateur</p>
                        </div>
                    </Reminder> 
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
        z-index: 100;
    }
}
@media screen and (max-width: 750px) {
    main {
        display: flex;
        flex-direction: column;
    }
}
</style>