<template>
    <div class="qcm">
        <div class="centrer">
            <h1 id="connaissances">TEST DE CONNAISSANCES </h1>
        </div>
        <br>
        <div class="decalement_QCM">
            <h3 id="gras"> Qu'est ce qu'un entretien ? </h3>
            
            <div class="inter_decalement">
                <label class="container"> 
                    L'entretien consiste simplement à aller voir des personnes qui pourrait potentiellement être intéressé par le produit que vous êtes en train de construire et à lui poser des questions.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>                    
                </label>
            
                <br>

                <label class="container"> 
                    L'entretien consiste à préserver la qualité d'un produit. Nous passons par l'étape de nettoyage puis de séchage.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>

                <br>

                <label class="container">
                    L'entretien est l'action de tenir, de conserver en bon état :travaux, dépenses nécessaires pour y parvenir.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>

            </div>

            <h3 id="gras"> Pourquoi faire des personas est important ? </h3>

            <div class="inter_decalement">
                <label class="container">
                    Définir un persona sert à comprendre le comportement de vos clients et potentiels prospects sur les canaix digitaux
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>

                <br>

                <label class="container">
                    Définir un persona permet au client de se rendre compte de quels couleurs le site sera fait.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
        
                <br>
                <label class="container">
                Définir un persona est important car il nous permet de définir la typographie.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>

                </label>
            </div>

            <h3 id="gras"> Que permet une expérience map ? </h3>

            <div class="inter_decalement">
                <label class="container">
                    Une expérience map permet de nous donner le plan du projet.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
        
                <br>
                
                <label class="container">
                    Il faut que l'employé ait une expérience map pour pouvoir effectuer le projet.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
        
                <br>
                <label class="container">
                    Une expérience map permet de mieux appréhender les actions de l'utilisateur pour lui proposer une interface adapté.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
            </div>

            <h3 id="gras"> Donner l'un des avantages de l'observation ? </h3>

            <div class="inter_decalement">
                <label class="container">
                    L'un des avantages de l'observation permet d'observer les employer afin de regarder ou ils en sont dans leurs travaux.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
                
                <br>
                
                <label class="container">
                    Récupérer les données par l'observation permet de faire émerger le non-verbal et les problématiques insoupçonnées auxquelles doit faire face le client dans son environnement naturel.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
                
                <br>
                
                <label class="container">
                    Permet de connaitre l'avancé du travail à faire.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                  </label>

            </div>

            <h3 id="gras"> Le focus group consiste en quoi ?</h3>

            <div class="inter_decalement">
                <label class="container">
                    Le Focus groupe consiste à se focaliser sur une seul et même tâche dans le groupe ( maquettage du site internet).
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>

                <br>
                
                <label class="container">
                    Le Focus groupe consiste à regrouper des personnes que vous aurez ciblé afin de discuter des points que vous aurez définis afvec votre équipe.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
                
                <br>
                <label class="container">
                    Le focus groupe a pour but d'évaluer la première impression que donne notre interface.
                    <input type="radio" name="radio">
                    <span class="checkmark"></span>
                </label>
            </div>

            <br>
            
            <button id="button" >VALIDER VOS REPONSES</button>
        </div>
    </div>
</template>

<script>
export default {
    
}

</script>

<style lang="scss">

.centrer {
    text-align: center;
}
#connaissances{
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
#button {
  background-color: #3F3D56;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
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
  background-color: #3F3D56;
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

</style>