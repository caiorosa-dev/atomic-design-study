<template>
	<a :href="to">
		<h3 class="nav-item">{{ text }}</h3>
	</a>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
	props: {
		text: {
			required: true,
			type: String
		},
		to: {
			required: true,
			type: String
		}
	}
});
</script>

<style lang="scss" scoped>
a {
	text-decoration: none;

	.nav-item {
		color: #293947;
		font-size: 1.3rem;
		transition: color 0.5s;

		&:hover {
			color: #ff895f;
		}
	}
}
</style>
