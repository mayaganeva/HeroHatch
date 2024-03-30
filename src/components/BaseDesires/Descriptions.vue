<script setup lang="ts">
defineProps(['desires']);
</script>

<template>
	<ul>
		<li v-for="desire in desires">{{ desire.name }}</li>
	</ul>
</template>
