<template>
	<nav class="nav-bar">
		<NavItem text="Serviços" to="/" />
		<NavItem text="Sobre Mim" to="/" />
		<NavItem text="Cases" to="/" />
		<NavItem text="Contato" to="/" />
	</nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { NavItem } from '@/components/atoms/';

export default defineComponent({
	components: { NavItem }
});
</script>

<style lang="scss" scoped>
.nav-bar {
	width: max-content;
	display: grid;
	grid-auto-flow: column;
	grid-gap: 2.5rem;
}
</style>
