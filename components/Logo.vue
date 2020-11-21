<template>
	<a
		:class="classList"
		class="no-underline hover:no-underline font-bold text-2xl lg:text-4xl"
		href="#"
	>
		<div class="flex justify-center items-center">
			<img src="@/assets/img/logo.png" alt="" class="w-16">
			<div class="ml-3">Team Mahal</div>
		</div>
	</a>
</template>

<script>
export default {
	name: 'Logo',
	props: {
		isStickable: {
			type: Boolean,
			default: false
		},
		isSticky: {
			type: Boolean,
			default: false
		}
	},
	computed: {
		classList() {
			let classList = ''
			if (this.isStickable) {
				classList = this.isSticky ? 'text-gray-800' : 'text-white'
			} else {
				classList = 'text-orange-600'
			}
			return classList
		}
	}
}
</script>