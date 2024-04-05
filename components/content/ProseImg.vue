<script lang="ts" setup>
const props = defineProps({
	src: {
		type: String,
		default: undefined,
	},
});
</script>

<template>
	<h6>ProseImg</h6>
	<NuxtImg id="xxx" :src="props.src" width="1000" sizes="100vw sm:50vw" format="webp" placeholder />
</template>

<style scoped>
img {
	border: 5px solid gold;
}
</style>
