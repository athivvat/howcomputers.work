<!-- ChapterIcon.svelte -->
<script lang="ts">
	export let iconType: string;
	export let color: string = '#2563eb';
</script>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 200 180" class="h-full w-full">
	{#if iconType === 'introduction'}
		<!-- Introduction to Computers -->
		<rect
			x="20"
			y="20"
			width="160"
			height="140"
			rx="10"
			fill="#f0f0f0"
			stroke={color}
			stroke-width="2"
		/>
		<rect x="40" y="40" width="120" height="70" rx="5" fill={color} />
		<rect x="60" y="120" width="80" height="20" rx="5" fill={color} opacity="0.7" />
		<circle cx="150" cy="55" r="8" fill="#fff" />
	{:else if iconType === 'binary'}
		<!-- Binary and Data -->
		<rect
			x="20"
			y="20"
			width="160"
			height="140"
			rx="10"
			fill="#f0f0f0"
			stroke={color}
			stroke-width="2"
		/>
		<text x="45" y="70" font-family="monospace" font-size="24" fill={color}>01</text>
		<text x="85" y="100" font-family="monospace" font-size="24" fill={color}>10</text>
		<text x="125" y="130" font-family="monospace" font-size="24" fill={color}>01</text>
		<circle cx="150" cy="40" r="8" fill={color} />
	{:else if iconType === 'architecture'}
		<!-- Computer Architecture -->
		<rect
			x="20"
			y="20"
			width="160"
			height="140"
			rx="10"
			fill="#f0f0f0"
			stroke={color}
			stroke-width="2"
		/>
		<rect
			x="50"
			y="50"
			width="100"
			height="80"
			rx="5"
			fill="none"
			stroke={color}
			stroke-width="2"
		/>
		<path
			d="M50 70 H150 M70 50 V130 M90 50 V130 M110 50 V130 M130 50 V130"
			stroke={color}
			stroke-width="2"
			opacity="0.5"
		/>
		<circle cx="150" cy="35" r="8" fill={color} />
	{:else if iconType === 'os'}
		<!-- Operating Systems -->
		<rect
			x="20"
			y="20"
			width="160"
			height="140"
			rx="10"
			fill="#f0f0f0"
			stroke={color}
			stroke-width="2"
		/>
		<rect x="40" y="40" width="120" height="25" rx="5" fill={color} />
		<rect x="40" y="75" width="55" height="65" rx="5" fill={color} opacity="0.7" />
		<rect x="105" y="75" width="55" height="65" rx="5" fill={color} opacity="0.4" />
		<circle cx="150" cy="35" r="8" fill="#fff" />
	{:else if iconType === 'networking'}
		<!-- Networking -->
		<rect
			x="20"
			y="20"
			width="160"
			height="140"
			rx="10"
			fill="#f0f0f0"
			stroke={color}
			stroke-width="2"
		/>
		<circle cx="70" cy="60" r="15" fill={color} />
		<circle cx="130" cy="60" r="15" fill={color} />
		<circle cx="70" cy="120" r="15" fill={color} />
		<circle cx="130" cy="120" r="15" fill={color} />
		<path
			d="M70 60 L130 60 L130 120 L70 120 L70 60 M70 60 L130 120 M130 60 L70 120"
			stroke={color}
			stroke-width="2"
			fill="none"
		/>
		<circle cx="150" cy="35" r="8" fill={color} />
	{:else}
		<!-- Future of Computing -->
		<rect
			x="20"
			y="20"
			width="160"
			height="140"
			rx="10"
			fill="#f0f0f0"
			stroke={color}
			stroke-width="2"
		/>
		<path
			d="M100 45 C140 45, 140 135, 100 135 C60 135, 60 45, 100 45"
			fill="none"
			stroke={color}
			stroke-width="2"
		/>
		<path d="M70 90 H130 M100 60 V120" stroke={color} stroke-width="2" />
		<circle cx="100" cy="90" r="25" fill="none" stroke={color} stroke-width="2" />
		<circle cx="100" cy="90" r="5" fill={color} />
		<circle cx="150" cy="35" r="8" fill={color} />
	{/if}
</svg>
