<template>
	<header class="header">
		<Logo />
		<NavBar />
		<SearchInput />
	</header>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { Logo } from '@/components/atoms';
import { NavBar, SearchInput } from '@/components/molecules/';

export default defineComponent({
	components: { Logo, NavBar, SearchInput }
});
</script>

<style lang="scss" scoped>
.header {
	display: grid;
	grid-template-columns: auto 1fr auto;
	grid-gap: 1rem;

	width: 100%;
	justify-items: center;
	align-items: center;
}
</style>
