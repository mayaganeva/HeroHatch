<script setup lang="ts">
defineProps(['title']);
</script>

<template>
	<div class="desire">
		<h3 class="subtitle">{{ title }}</h3>
		<ul></ul>
		<button>Add random</button>
	</div>
</template>
