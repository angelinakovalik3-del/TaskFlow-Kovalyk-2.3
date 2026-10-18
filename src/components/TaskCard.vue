
<template>
  <div class="task-card">
    <div class="task-card__top">
      <span
        class="task-status"
        :class="`status-${task.status}`"
      >
        {{ statusText }}
      </span>

      <span
        class="task-priority"
        :class="`priority-${task.priority}`"
      >
        {{ priorityText }}
      </span>
    </div>

    <h3 class="task-card__title">{{ task.title }}</h3>
    <p class="task-card__description">{{ task.description }}</p>
  </div>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps({
  task: {
    type: Object,
    required: true,
  },
});

const statusText = computed(() => ({
  todo: 'Заплановано',
  progress: 'У роботі',
  done: 'Виконано',
}[props.task.status] ?? props.task.status));

const priorityText = computed(() => ({
  low: 'Низький',
  medium: 'Середній',
  high: 'Високий',
}[props.task.priority] ?? props.task.priority));
</script>
