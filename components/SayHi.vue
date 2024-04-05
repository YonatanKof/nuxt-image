<script lang="ts" setup>
const props = defineProps({
	src: {
		type: String,
		default: undefined,
	},
});
</script>

<template>
	<h6>SayHi</h6>
	<NuxtImg :src="props.src" width="1000" sizes="100vw sm:50vw md:400px" format="webp" placeholder />
</template>

<style scoped>
img {
	border: 5px solid lawngreen;
}
</style>
