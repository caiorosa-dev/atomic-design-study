<template>
	<div class="social-networks">
		<SocialLink icon="facebook.svg" to="https://github.com/bug4do" />
		<SocialLink icon="github.svg" to="https://github.com/bug4do" />
		<SocialLink icon="twitter.svg" to="https://github.com/bug4do" />
	</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

import { SocialLink } from '@/components/atoms';

export default defineComponent({
	components: { SocialLink }
});
</script>

<style lang="scss" scoped>
.social-networks {
	display: grid;
	grid-gap: 1rem;
}
</style>
