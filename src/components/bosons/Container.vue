<template>
	<div class="container">
		<slot />
	</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({});
</script>

<style lang="scss" scoped>
.container {
	width: 85%;
	margin: 0 auto;
	max-width: 1150px;
}
</style>
