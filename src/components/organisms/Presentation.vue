<template>
	<section class="presentation">
		<SocialNetworks />
		<img class="presentation-img" src="@/assets/images/presentation.svg" alt="Presentation" />
	</section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { SocialNetworks } from '@/components/molecules/';

export default defineComponent({
	components: { SocialNetworks }
});
</script>

<style lang="scss" scoped>
.presentation {
	display: grid;
	justify-content: center;
	grid-template-columns: auto 1fr;
	align-items: center;

	.presentation-img {
		width: 70%;
		justify-self: center;
	}
}
</style>
