<template>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-5 px-8">
    <MealItem
      v-for="meal of meals"
      :key="meal.idMeal"
      :meal="meal"
      class="bg-blue shadow rounded"
    />
  </div>

  <div v-if="!meals.length" class="flex justify-center text-gray-600 p-8">
    No Meals Found
  </div>
</template>

<script setup>
import MealItem from "./MealItem.vue";

const { meals } = defineProps({
  meals: {
    required: true,
    type: Array,
  },
});
</script>

<style scoped></style>
