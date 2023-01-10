<template>
	<section class="services">
		<Service title="Front-End" description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptate dolor iure saepe vel nihil mollitia ad numquam, hic laudantium est officia qui fugit pariatur impedit. Accusamus sapiente dolore soluta pariatur." />
		<Service title="Back-End" description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptate dolor iure saepe vel nihil mollitia ad numquam, hic laudantium est officia qui fugit pariatur impedit. Accusamus sapiente dolore soluta pariatur." />
		<Service title="UI/UX Design" description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptate dolor iure saepe vel nihil mollitia ad numquam, hic laudantium est officia qui fugit pariatur impedit. Accusamus sapiente dolore soluta pariatur." />
	</section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { Service } from '@/components/molecules/';

export default defineComponent({
	components: { Service }
});
</script>

<style lang="scss" scoped>
.services {
	display: grid;
	grid-template-columns: repeat(3, 1fr);
	grid-gap: 5rem;
}
</style>
