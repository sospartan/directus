<template>
	<div class="v-sheet">
		<slot />
	</div>
</template>

<style lang="scss" scoped>
/*

	Available Variables:

		--v-sheet-background-color  [var(--background-subdued)]
		--v-sheet-height            [auto]
		--v-sheet-min-height        [var(--input-height)]
		--v-sheet-max-height        [none]
		--v-sheet-width             [auto]
		--v-sheet-min-width         [none]
		--v-sheet-max-width         [none]
		--v-sheet-padding           [8px]

*/

.v-sheet {
	width: var(--v-sheet-width, auto);
	min-width: var(--v-sheet-min-width, none);
	max-width: var(--v-sheet-max-width, none);
	height: var(--v-sheet-height, auto);
	min-height: var(--v-sheet-min-height, var(--input-height));
	max-height: var(--v-sheet-max-height, none);
	padding: var(--v-sheet-padding, 8px);
	overflow: auto;
	background-color: var(--v-sheet-background-color, var(--background-subdued));
	border-radius: var(--theme--border-radius);
}
</style>
