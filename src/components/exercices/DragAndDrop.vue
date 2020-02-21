<template>
    <section class="draganddrop">
        <div class="big-title-box">
                <h1 class="big-title">Drag And Drop'</h1>
        </div>
        <p class="rules">Le but du jeu est de remettre les élements dans le bon ordre, dans les bonnes cases.</p>
        <div class="drag-container">
            <div class="cards-box default-cards-box">
            <draggable class="list-group" tag="ul" v-model="list" v-bind="dragOptions" :move="onMove" @start="isDragging=true" @end="isDragging=false">
                <transition-group type="transition" :name="'flip-list'">
                <li class="list-group-item" v-for="element in list" :key="element.order">
                    <i :class="element.fixed? 'fa fa-anchor' : 'glyphicon glyphicon-pushpin'" @click=" element.fixed=! element.fixed" aria-hidden="true"></i>
                    {{element.name}}
                    <span class="badge">{{element.order}}</span>
                </li>
                </transition-group>
            </draggable>
            </div>

            <div class="cards-box final-cards-box">
                <ul class="cards-label">
                    <li class="card-label"  v-for="label in cardsLabel" :key="label">{{label}}</li>
                </ul>
                <draggable element="span" v-model="list2" v-bind="dragOptions" :move="onMove">
                    <transition-group name="no" class="list-group" tag="ul">
                    <li class="list-group-item" v-for="element in list2" :key="element.order">
                        <i :class="element.fixed? 'fa fa-anchor' : 'glyphicon glyphicon-pushpin'" @click=" element.fixed=! element.fixed" aria-hidden="true"></i>
                        {{element.name}}
                        <span class="badge">{{element.order}}</span>
                    </li>
                    </transition-group>
                </draggable>
            </div>
        </div>
        <div class="validation-box">
            <button class="button" id="button" >VALIDER VOS REPONSES</button>
        </div>
    </section>
</template>

<script>
import draggable from "vuedraggable";
const message = [
  "Etablir un lieu propre et chaleureux",
  "Accueillir les participants agréablement",
  "Définir les règles",
  "Emettre les idées de façon respectueuse",
  "Faire un bilan"
];
export default {
  name: "hello",
  components: {
    draggable
  },
  data() {
    return {
      list: message.map((name, index) => {
        return { name, order: index + 1, fixed: false };
      }),
      list2: [],
      editable: true,
      isDragging: false,
      delayedDragging: false,
      cardsLabel: ["1","2","3","4","5"]
    };
  },
  methods: {
    orderList() {
      this.list = this.list.sort((one, two) => {
        return one.order - two.order;
      });
    },
    onMove({ relatedContext, draggedContext }) {
      const relatedElement = relatedContext.element;
      const draggedElement = draggedContext.element;
      return (
        (!relatedElement || !relatedElement.fixed) && !draggedElement.fixed
      );
    }
  },
  computed: {
    dragOptions() {
      return {
        animation: 0,
        group: "description",
        disabled: !this.editable,
        ghostClass: "ghost"
      };
    }
  },
  watch: {
    isDragging(newValue) {
      if (newValue) {
        this.delayedDragging = true;
        return;
      }
      this.$nextTick(() => {
        this.delayedDragging = false;
      });
    }
  }
};
</script>

<style lang="scss" scoped>
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

section.draganddrop {
    min-height: 100vh;
    max-width: 1100px;
    padding: 20px;
    width: 100%;
    margin: 0 auto;

    p.rules {
        margin: 40px 0;
        font-weight: 700;
        font-size: 1.2em;
    }
}
.drag-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    column-gap: 1rem;

    @media screen and (max-width: 900px) {
        & {
            grid-template-columns: 1fr;
            grid-row-gap: 1rem;
        }
    }

    ul {
        height: 100%;
        list-style: none;
    }

    .list-group-item, .final-cards-box li{
        font-family: "Lato", sans-serif;
        font-size: 1.2em;
        font-weight: 500;
        background-color: #3F3D56;
        padding: 10px 15px;
        color: white;
        margin: 10px 0;
    }
    .cards-box {
        padding: 10px;
        border: 1px solid #3F3D56;
    }
    .final-cards-box {
        display: flex;
        li {
            margin-right: 5px;  
        }

        span {
            flex: 1;
        }


    }
}

.validation-box {
    text-align: center;
}


.flip-list-move {
  transition: transform 0.5s;
}
.no-move {
  transition: transform 0s;
}
.ghost {
  opacity: 0.5;
  background: #c8ebfb;
}
.list-group {
  min-height: 20px;
}
.list-group-item {
  cursor: move;
}
.list-group-item i {
  cursor: pointer;
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
    margin: 20px auto;
    transition-duration: .2s;
    cursor: pointer;

    &:hover {
        background-color: #555275;
        transform: scale(0.97)
    }
}

</style>