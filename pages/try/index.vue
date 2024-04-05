<script setup>
const { data } = await useAsyncData('equal', () => {
	return queryContent('try').where({}).find();
});
</script>

<template>
	<section>
		<div v-for="(item, index) in data" :key="index">
			<NuxtLink :to="item._path" style="text-decoration: none">
				<h3>{{ item.title }}</h3>
				<SayHi :src="item.image" />
			</NuxtLink>
		</div>
		<SayHi src="/try/dove-1.jpg" />
	</section>
</template>
<style scoped>
div {
	border: 5px solid red;
}
</style>
