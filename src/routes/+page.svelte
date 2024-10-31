<script lang="ts">
	let displayText = 'How Computers Work?';
	let cursorVisible = true;

	setInterval(() => {
		cursorVisible = !cursorVisible;
	}, 500);
</script>

<div class="flex min-h-screen items-center justify-center bg-black text-green-500">
	<div class="flex items-center font-mono">
		<span>{displayText}</span>
		<div class="w-10 -mt-0.5">
            <span class={cursorVisible ? 'inline-block' : 'hidden'}>|</span>
		</div>
	</div>
</div>
