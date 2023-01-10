<template>
	<div id="app">
		<HomeTemplate />
	</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

import HomeTemplate from './components/templates/HomeTemplate.vue';

export default defineComponent({
	name: 'App',
	components: { HomeTemplate }
});
</script>
