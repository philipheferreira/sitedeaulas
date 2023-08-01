<template>
  <div class="column">
    <div class="q-ma-md column items-center">
      <!--<p class=" info">Aulas do professor Milton Oliveira postadas no canal
        do youtube e compartilhadas neste reposritorio</p>-->
    </div>
    <div class="row q-ma-md">
      <card-aula site="https://www.youtube.com/embed/iumsSe2783I" titulo="Aula 01" autor="By Prof. Milton Oliveira"
        sobre="O estudo não depende somente do material que escolhe e das horas que disponibiliza. Seja mais eficiente no estudo da matemática"></card-aula>

      <card-aula site="https://www.youtube.com/embed/GrqMumngTvc" titulo="Aula 02" autor="By Prof. Milton Oliveira"
        sobre="Essa questão causa dificuldade quando estamos acostumado a achar ângulo por ângulo para realizar as operações com eles, nessa questão é um pouco diferente"></card-aula>

      <card-aula site="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" titulo="Aula 03" autor="By Prof. Milton Oliveira"
        sobre="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua."></card-aula>

      <card-aula site="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" titulo="Aula 04" autor="By Prof. Milton Oliveira"
        sobre="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua."></card-aula>

      <card-aula site="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" titulo="Aula 05" autor="By Prof. Milton Oliveira"
        sobre="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua."></card-aula>
    </div>
  </div>
</template>

<script>
import cardAula from "components/CardAula.vue"

export default {
  components: {
    cardAula
  }
}
</script>

<style scoped>
.my-card {
  width: 100%;
  max-width: 300px;
}

.info {
  padding: 0px 20px;
  border: 1px solid #cccccc;
  border-radius: 15px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
}
</style>
