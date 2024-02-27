<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->

<div class="container mx-auto h-full flex justify-center items-center">
	<div class="fig">
		<div class="card w-full p-4 m-4">
			<div class="img-bg"></div>
			<div class="card-header">
				<span>Something to do:</span>
				<input type="text" class="input" placeholder="thing to do" />
				<div class="flex flex-row-reverse mt-4">
					<button class="btn variant-filled-primary">Get Started</button>
				</div>
			</div>
		</div>
	</div>
</div>

<style lang="postcss">
	.fig {
		@apply flex relative flex-col;
	}
	.fig .tin,
	.img-bg {
		@apply w-64 h-64 md:w-80 md:h-20;
	}
	.img-bg {
		@apply absolute z-[-1] rounded-full blur-[70px] transition-all;
		animation:
			pulse 5s cubic-bezier(0, 0, 0, 0.5) infinite,
			glow 5s linear infinite;
	}
	@keyframes glow {
		0% {
			@apply bg-primary-400/50;
		}
		33% {
			@apply bg-secondary-400/50;
		}
		66% {
			@apply bg-tertiary-400/50;
		}
		100% {
			@apply bg-primary-400/50;
		}
	}
	@keyframes pulse {
		50% {
			transform: scale(1.5);
		}
	}
</style>
