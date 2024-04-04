<script lang="ts" setup>
const props = defineProps({
	src: {
		type: String,
		default: '',
	},
});
</script>

<template>
	<NuxtImg id="xxx" :src="props.src" width="1000" sizes="100vw sm:50vw" format="webp" placeholder />
</template>

<style scoped>
#xxx {
	border: 5px solid red;
}
</style>
