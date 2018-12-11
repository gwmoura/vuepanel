<template>
  <div id="Panel">
    Painel de Perguntas
    <div v-for="question in questions">
    {{ question }}
  </div>
    <PanelCard
      v-for="(question, index) in questions"
      v-bind:question="question"
      v-bind:index="index"
      v-bind:key="item.id"
      />
  </div>
</template>

<script>
import PanelCard from './PanelCard'

export default {
  name: 'Panel',
  data: {
    questions: [
      {
        id: 1,
        question: 'Uma pergunta?',
        options: [{id: 1, label: 'Sim'}, {id: 2, label: 'Não'},]
      }
    ]
  },
  components: {
    PanelCard
  }
}
</script>

<style>
</style>
