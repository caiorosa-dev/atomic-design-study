<template>
	<form class="search-input">
		<input type="search" placeholder="Buscar" />

		<button type="submit">
			<img src="@/assets/images/icons/search.svg" alt="Buscar" />
		</button>
	</form>
</template>

<style lang="scss" scoped>
.search-input {
	position: relative;
	width: max-content;
	transition: all 0.5s;

	input {
		border: none;
		border-radius: 1rem;
		padding: 0.5rem 1rem;
		box-shadow: 0px 5px 5px rgba(#000000, 0.08);
		font-family: 'Lato';

		&::placeholder {
			color: #a9b0be;
		}
	}

	button {
		position: absolute;
		right: 3px;
		top: 50%;
		transform: translateY(-50%);

		width: 30px;
		height: 30px;

		display: grid;
		justify-items: center;
		align-items: center;

		background: #ff895f;
		border: none;
		border-radius: 5rem;

		&:hover {
			cursor: pointer;
			background: #ff7746;
		}
	}
}
</style>
