<template>
	<a :href="to" class="social-link" target="_blank">
		<img :src="iconPath" :alt="icon" />
	</a>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
	props: {
		icon: {
			required: true,
			type: String
		},
		to: {
			required: true,
			type: String
		}
	},
	computed: {
		iconPath(): string {
			return require(`@/assets/images/icons/${this.icon}`);
		}
	}
});
</script>

<style lang="scss" scoped>
.social-link {
	background-color: #ff895f;
	width: 47px;
	height: 47px;
	border-radius: 5rem;
	display: grid;
	justify-items: center;
	align-items: center;
	transition: transform 0.25s linear;

	&:hover {
		transform: scale(1.1);
	}

	img {
		width: 23px;
		height: 23px;
	}
}
</style>
