<script setup lang="ts">
import { ref } from 'vue';

// defineProps<{ msg: string }>();
// defineProps({
// 	msg: {
// 		type: String,
// 		default: '',
// 	},
// });
defineProps<{
	// 采用ts专有声明，无默认值
	msg?: string;
	num?: number;
}>();

const count = ref(0);
</script>

<template>
	<h1>{{ msg }}</h1>
	<div></div>

	<!-- <div class="card">
		<button type="button" @click="count++">count is {{ count }}</button>
	</div> -->
</template>

<style scoped>
.read-the-docs {
	color: #888;
}
</style>
