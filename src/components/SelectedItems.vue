<template>
  <div class="selected-items">
    <h3>{{ title }}</h3>
    <ul>
      <li v-for="item in items" :key="item.id" class="selected-items__item">
        {{ item.name }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    items: {
      type: Array,
      default: () => []
    },
    title: {
      type: String,
      default: null
    }
  }
}
</script>

<style scoped></style>
