<template>
  <div id="PanelCard">
    <div class="PanelCardQuestion">{{ question }}</div>
    <div class="PanelCardOptions">
        <ul>
            <li
            is="option-item"
            v-for="(option) in options"
            v-bind:key="option.id"
            v-bind:label="option.label"
            ></li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PanelCard',
  porps: {
    question: String,
    options: Array
  }
}
</script>

<style>
</style>
