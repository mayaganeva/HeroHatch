<script setup lang="ts">
import Container from './Container.vue';
import Descriptions from './Descriptions.vue';

const desires = [
	{
		name: 'honor',
		short: 'I feel proud that my personal values are reflected in my actions',
		tendencies: {
			high: 'experience shame and guilt when they fail or neglect their duty',
			low: 'less shame / guilt',
		},
	},
	{
		name: 'status',
		short: 'My position is good, and recognized by the people around me',
		tendencies: {
			high: 'The driven by status want to go "up" in the world, become "somebody". Impressed by fame, care about reputation, may feel important or even superior. They enjoy the attention. ',
			low: "Unimpressed by expensive things or celebrities. Don't care so much about their reputation.",
		},
	},
	{
		name: 'tranquility',
		short: "I don't experience unhealthy amounts of stress",
		tendencies: {
			high: "Managing stress can become limiting (don't want to go out) or lead to substance abuse. Correlates to low tolerance for pain or a high number of fears.",
			low: "Self-confidence may be the reason some people experience less stress, but doesn't mean they actually want stress. Percieve stress as a temporary nuisance.",
		},
	},
];
</script>

<template>
	<h2 class="title">Base Desires</h2>
	<p>Short info about what base desires represent and how to use them in RP</p>
	<div class="desires">
		<Container title="High" />
		<Container title="Low" />
	</div>
	<Descriptions :desires="desires" />
</template>
