<template>
  <div id="app">
    <button class="row" @click="rowDice">Row!</button>
    <transition name="drop">
      <component :is="point" :point="number"></component>
    </transition>
    <!-- <p class="point">Point : {{showNumber}} 
    </p> -->
  </div>
</template>

<script>
import Dice from "./components/Dice.vue";
import Dice1 from "./components/Dice1.vue";
import Dice2 from "./components/Dice2.vue";
import Dice3 from "./components/Dice3.vue";
import Dice4 from "./components/Dice4.vue";
import Dice5 from "./components/Dice5.vue";
import Dice6 from "./components/Dice6.vue";

export default {
  data() {
    return {
      number: "",
      showNumber: ""
    };
  },
  methods: {
    rowDice() {
      let number = Math.floor(Math.random() * 6 + 1);
      this.number = number;
      setTimeout(() => {
        this.showNumber = number;
      }, 2000);
      // console.log(this.number);
    }
  },
  computed: {
    point() {
      if (this.number === 1) {
        return "app-dice1";
      } else if (this.number === 2) {
        return "app-dice2";
      } else if (this.number === 3) {
        return "app-dice3";
      } else if (this.number === 4) {
        return "app-dice4";
      } else if (this.number === 5) {
        return "app-dice5";
      } else if (this.number === 6) {
        return "app-dice6";
      } else {
        return "app-dice";
      }
    }
  },
  components: {
    appDice: Dice,
    appDice1: Dice1,
    appDice2: Dice2,
    appDice3: Dice3,
    appDice4: Dice4,
    appDice5: Dice5,
    appDice6: Dice6
  }
};
</script>

<style scoped>
#app {
  width: 600px;
  height: 600px;
  margin: 0 auto;
  background: #f5f5f5;
  display: flex;
  justify-content: center;
  position: relative;
  /* perspective: 300px; */
}

.row {
  font-size: 20px;
  width: 75px;
  height: 50px;
  position: absolute;
  top: 20px;
  left: 20px;
  border: 1px solid black;
  border-radius: 5px;
  background: aquamarine;
  outline: none;
}

.point {
  padding: 0;
  margin: 0;
  height: 30px;
  line-height: 30px;
  position: absolute;
  top: 20px;
  left: 100px;
}

.drop-enter {
}

.drop-enter-active {
}

.drop-leave {
}

.drop-leave-active {
  display: none;
}
</style>
