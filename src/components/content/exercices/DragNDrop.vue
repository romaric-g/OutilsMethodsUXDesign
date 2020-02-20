<template>
    <div class="content">
        <h1>DRAG AND DROP'</h1>
        <p>Le but du jeu est de remettre les éléments dans le bon ordre, dans les bonnes cases.</p>
        <ul>
            <li id="element1">Etablir un lieu propre et chaleureux</li>
            <li id="element2">Etablir un lieu propre et chaleureux</li>
            <li id="element3">Etablir un lieu propre et chaleureux</li>
            <li id="element4">Etablir un lieu propre et chaleureux</li>
            <li id="element5">Etablir un lieu propre et chaleureux</li>
        </ul>
        <ul>
            <li id="answer1">1</li>
            <li id="answer1">2</li>
            <li id="answer1">3</li>
            <li id="answer1">4</li>
            <li>5</li>
        </ul>
        <button>VALIDER VOS REPONSES</button>
////////////////////////////////////////////////////////////////
        <p>Drag the W3Schools image into the rectangle:</p>

        <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
        <br>
        <p id="drag1" draggable="true" ondragstart="drag(event)" width="336" height="69">blablabla </p>
/////////////////////////////////////////////////////////////////
    </div>
</template>

<script>
/////////////////////////////////////////////////////////////////
        function allowDrop(ev) {
  ev.preventDefault();
}

function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.id);
}

function drop(ev) {
  ev.preventDefault();
  var data = ev.dataTransfer.getData("text");
  ev.target.appendChild(document.getElementById(data));
}
/////////////////////////////////////////////////////////////////

export default {
    
}
</script>

<style lang="scss">
#div1 {
  width: 350px;
  height: 70px;
  padding: 10px;
  border: 1px solid #aaaaaa;
}
</style>