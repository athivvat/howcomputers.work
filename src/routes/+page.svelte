<script lang="ts">
	import ChapterIcon from '../components/icons/ChapterIcon.svelte';

	let chapters = [
		{
			title: 'Introduction to Computers',
			description:
				'Learn the basic concepts of computers, including hardware, software, and how theyinteract.',
			iconType: 'introduction',
			color: '#d4d4d4',
			contents: [
				{
					title: 'History of Computers',
					description: 'Explore the evolution of computers from the abacus to modern devices.'
				}
			]
		},
		{
			title: 'Binary and Data Representation',
			description:
				'Understand how computers use binary numbers to represent data and perform calculations.',
			iconType: 'binary',
			color: '#d4d4d4',
			contents: [
				{
					title: 'History of Computers',
					description: 'Explore the evolution of computers from the abacus to modern devices.'
				}
			]
		},
		{
			title: 'Computer Architecture',
			description:
				'Explore the fundamental components of a computer system, including the CPU, memory, and I/O devices.',
			iconType: 'architecture',
			color: '#d4d4d4',
			contents: [
				{
					title: 'History of Computers',
					description: 'Explore the evolution of computers from the abacus to modern devices.'
				}
			]
		},
		{
			title: 'Operating Systems',
			description:
				'Learn about the role of operating systems in managing hardware and software resources.',
			iconType: 'os',
			color: '#d4d4d4',
			contents: [
				{
					title: 'History of Computers',
					description: 'Explore the evolution of computers from the abacus to modern devices.'
				}
			]
		},
		{
			title: 'Networking and the Internet',
			description:
				'Discover how computers communicate with each other over networks and the internet.',
			iconType: 'networking',
			color: '#d4d4d4',
			contents: [
				{
					title: 'History of Computers',
					description: 'Explore the evolution of computers from the abacus to modern devices.'
				}
			]
		},
		{
			title: 'Future of Computing',
			description: 'Explore emerging technologies and the future trends in computing.',
			iconType: 'future',
			color: '#d4d4d4',
			contents: [
				{
					title: 'History of Computers',
					description: 'Explore the evolution of computers from the abacus to modern devices.'
				}
			]
		}
	];
</script>

<div class="pt-12">
	<div class="mb-6 border-b border-t">
		<div class="container max-w-screen-lg py-2">
			<h1 class="font-mono text-xs uppercase tracking-widest">How Computers Work?</h1>
		</div>
	</div>
	<div class="mb-6 border-b border-t">
		<div class="container max-w-screen-lg py-2">
			<h1 class="text-5xl font-semibold">Build computers from scratch</h1>
			<p>The best way to understand how computers work is to build one from scratch</p>
		</div>
	</div>
	<div class="border-b border-t">
		<div class="container grid max-w-screen-lg md:grid-cols-6 grid-cols-2 p-0">
			{#each chapters as chapter}
				<a href="/" class="border-r p-4 text-center last:border-r-0 md:border-b-0 border-b last:border-b-0 second-last-child hover:bg-gray-100">
					<div class="flex flex-col items-center justify-center">
						<div class="mb-2 h-24 w-24">
							<ChapterIcon iconType={chapter.iconType} color={chapter.color} />
						</div>
						<div class="h-14">
							<h2 class="font-mono text-xs">{chapter.title}</h2>
						</div>
						<p class="sr-only">{chapter.description}</p>
					</div>
				</a>
			{/each}
		</div>
	</div>
	<div class="mb-6 border-b">
		<div class="container max-w-screen-lg py-12">
			<div class="prose mx-auto">
				<h2 class="text-2xl font-semibold">Preface</h2>
				<p>
					Welcome to "How Computers Work"! This guide is designed to take you on a journey through
					the fascinating world of computers. Whether you are a beginner or have some experience,
					this guide will provide you with a solid understanding of the fundamental concepts and
					components that make up a computer system.
				</p>
				<p>
					We will start with the basics, exploring the history and evolution of computers, and then
					delve into more complex topics such as binary data representation, computer architecture,
					operating systems, and networking. By the end of this guide, you will have a comprehensive
					understanding of how computers work and be well-equipped to build and troubleshoot your
					own computer systems.
				</p>
				<p>
					Let's embark on this exciting journey together and uncover the mysteries of computing!
				</p>
			</div>
		</div>
	</div>
</div>
