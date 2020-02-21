<template>
    <section class="qcm">
        <div class="centrer">
            <h1 id="connaissances">TEST DE CONNAISSANCES </h1>
        </div>
        <br>
        <div class="decalement_QCM" v-for="(question, index) in questionsList" :key="index">
            <h3 id="gras">{{ question.question }}</h3>
            
            <div class="inter_decalement" v-for="(answer, indexA) in question.answers" :key="indexA">
                <label class="container" :for="'answer-' + index + '-' + indexA" :class="getColorClass(index, indexA)"> 
                    {{ answer }}
                    <input :value="indexA" type="radio" :id="'answer-' + index + '-' + indexA" :name="'answer-' + index" v-model="answers[index]" :disabled="reveal">
                    <span class="checkmark" ></span>         
                </label>
                <br>
            </div>

            <br>
        </div>
        <button id="button" @click.prevent="revealAnswers" >VALIDER VOS REPONSES</button>
    </section>
</template>

<script>
export default {
    data() {
        return {
            questionsList: [
                {question: "Qu'est ce qu'un entretien ?", answers: ["L’entretien consiste simplement à aller voir des personnes qui pourrait potentiellement être intéressé par le produit que vous êtes en train de construire et à lui poser des questions.",
                                                                    "L’entretien consiste à préserver la qualité d’un produit. Nous passons par l’étape de nettoyage puis de séchage.",
                                                                    "L’entretien est l’action de tenir, de conserver en bon état ; travaux, dépenses nécessaires pour y parvenir."],
                                                                    response: 0
                },
                {question: "Pourquoi faire des personas est important ?",  answers: ["Définir un persona sert à comprendre le comportement de vos clients et potentiels prospects sur les canaux digitaux.",
                                                                    "Définir un persona permet au client de se rendre compte de quels couleurs le site sera fait.",
                                                                    "Définir un persona est important car il nous permet de définir la typographie."],
                                                                    response: 0
                },
                {question: "Que permet une expérience map ?",  answers: ["Une expérience map permet de nous donner le plan du projet.",
                                                                    "Il faut que l’employé ait une expérience map pour pouvoir effectuer le projet.",
                                                                    "Une expérience map permet de mieux appréhender les actions de l’utilisateur pour lui proposer une interface adapté."],
                                                                    response: 2
                },
                {question: "Donner l’un des avantages de l’observation",  answers: ["L’un des avantages de l’observation permet d’observer les employer afin de regarder ou ils en sont dans leurs travaux.",
                                                                    "Récupérer des données par l’observation permet de faire émerger le non-verbal et des problématiques insoupçonnées auxquelles doit faire face le client dans son environnement naturel.",
                                                                    "L’un des avantages de l’observation."],
                                                                    response: 1
                },
                {question: "Donner l’un des avantages de l’observation",  answers: ["Le Focus groupe consiste à se focaliser sur une seul et même tâche dans le groupe (maquettage du site internet)",
                                                                    "Le Focus groupe consiste à regrouper des personnes que vous aurez ciblé afin de discuter des points que vous aurez définis avec votre équipe.",
                                                                    "Le focus groupe a pour but d’évaluer la première impression que donne notre interface. "],
                                                                    response: 1
                }
            ],
            answers: [],
            reveal: false
        }
    },
    methods: {
        revealAnswers() {
            this.reveal = true;
        },
        getColorClass(questionID, answerID) {
            if(this.reveal) {
                let valueSet = this.answers[questionID];
                let question = this.questionsList[questionID];
                let response = question.response;
                if(valueSet == answerID) {
                    if(valueSet == response)return "valide";
                    else return "error";
                }else {
                    
                    if(answerID == response) {
                        return "valide";
                    }
                }
                return {
                    
                }
            }
        }
    }
}

</script>

<style lang="scss" scoped>
section.qcm {
    max-width: 1100px;
    padding: 20px;
    width: 100%;
    margin: 0 auto;

    .centrer {
        text-align: center;
    }
    #connaissances{
        font-family: "Montserrat", sans-serif;
        display: inline-block;
        text-align:center;
        position: relative; 
            &:after {
                content: "";
                position: absolute;
                bottom: -2px;
                height: 2px;
                left: 0;right: 0;
                background-color: black;
            }
    }

    #gras{
        font-weight : bold;
    }

    button {
        display: block;
        font-family: "Montserrat";
        font-weight: 700;
        font-size: 2em;
        color: white;
        background-color: #3f3d56;
        width: 280px;
        line-height: 1em;
        padding: 5px 0;
        border: none;
        margin: 0 auto;
        transition-duration: .2s;
        cursor: pointer;

        &:hover {
            background-color: #555275;
            transform: scale(0.97)
        }
    }

    .decalement_QCM{
        margin-left:10%;
        margin-right:10%;
    }
    .inter_decalement{
        margin-left:5%;
    }
    /* The container */
    .container {
    display: block;
    position: relative;
    padding-left: 25px;
    cursor: pointer;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
    }

    /* Hide the browser's default radio button */
    .container input {
    position: absolute;
    opacity: 0;
    cursor: pointer;
    }

    /* Create a custom radio button */
    .checkmark {
    position: absolute;
    top: 0;
    left: 0;
    height: 15px;
    width: 15px;
    background-color: #eee;
    border-radius: 50%;
    }

    /* On mouse-over, add a grey background color */
    .container:hover input ~ .checkmark {
    background-color: #ccc;
    }

    /* When the radio button is checked, add a blue background */
    .container input:checked ~ .checkmark {
    background-color: rgb(249, 168, 38);
    }

    /* Create the indicator (the dot/circle - hidden when not checked) */
    .checkmark:after {
    content: "";
    position: absolute;
    display: none;
    }

    /* Show the indicator (dot/circle) when checked */
    .container input:checked ~ .checkmark:after {
    display: block;
    }

    label{
        font-family: "Lato", sans-serif;
    }

    label.error {
        color: red;
    }

    label.valide {
        color: green;
        font-weight: 700;
    }

}
</style>