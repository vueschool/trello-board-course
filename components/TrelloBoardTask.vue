<script setup lang="ts">
import type { Task } from "@/types";
defineProps<{
  task: Task;
}>();
</script>
<template>
  <div
    :title="task.createdAt.toLocaleString()"
    class="task bg-white p-2 mb-2 rounded shadow-sm max-w-[250px]"
  >
    <span>
      {{ task.title }}
    </span>
  </div>
</template>
