<template>
  <div id="PanelCard">
    <div class="PanelCardQuestion">{{ question.question }}</div>
    <div class="PanelCardOptions">
        <ul>
            <li v-for="(option) in question.options">{{ option.label }}</li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PanelCard',
  props: {
    question: Object,
    options: Array
  }
}
</script>

<style>
</style>
