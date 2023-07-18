<template>
  <q-page class="">
    <div class="column items-center">
      <img alt="Quasar logo" src="https://www.unijui.edu.br/arquivos/tinyMCE4/comunica1/rotina%20de%20estudos%202023.png"
        style="height: 300px; width: 300px;" class="q-ma-md" />
      <p>Professor: Milton Oliveira</p>
    </div>
    <h5 class="text-center">sobre</h5>
    <div class="info text-center">
      <p>Estudo a um tempo como a matemática afeta a aprendizagem e sua importância dentro do estudo geral humano. Trabalho com meus alunos dentro da perspectiva de auxiliá-los no contato com a disciplina e aprimoramento pessoal</p>
      <p>Formação:Licencitura plena em matemática na UFPA em 2019</p>
    </div>
    <div class="q-pa-md">
      <q-table title="Disponibilidade de Horario" :rows="rows" :columns="columns" row-key="name" hide-bottom />
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

const columns = [
  {

    required: true,
    label: 'Segunda-Feira',
    align: 'center',
    field: (row) => row.name,
    format: (val) => `${val}`,
    sortable: true,
  },
  {
    name: 'Terça-feira', label: 'Terça-feira', field: 'fat', sortable: true,
  },
  { name: 'Quarta-feira', label: 'Quarta-feira', field: 'carbs' },
  { name: 'Quinta-feira', label: 'Quinta-feira', field: 'protein' },
  { name: 'Sexta-feira', label: 'Sexta-feira', field: 'sodium' },
  {
    name: 'Sabado', label: 'Sabado', field: 'calcium', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10),
  },
  {
    name: 'Domingo', label: 'Domingo', field: 'iron', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10),
  },
];

const rows = [
  {
    name: '14:00-15:00',
    fat: '14:00-15:00',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
  {
    name: '15:00-16:00',
    fat: '15:00-16:00',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
  {
    name: '-',
    fat: '16:00-17:00',
    carbs: '-',
    protein: '-',
    sodium: '16:00-17:00',
    calcium: '-',
    iron: '-',
  },
  {
    name: '-',
    fat: '-',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
  {
    name: '-',
    fat: '-',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
];

export default defineComponent({
  name: "PageIndex",
  setup() {
    return {
      columns,
      rows
    }
  }
});
</script>

<style>
  .info{
    margin: 5px 300px;
  }
</style>