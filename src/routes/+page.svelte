<script lang="ts">
	import * as Card from '$lib/components/ui/card/index';
	import profilePicture from '$lib/assets/profile-picture.png';
	import { Button } from '$lib/components/ui/button/index';
	import { Telescope } from 'lucide-svelte';
</script>

<div class="mb-8 flex w-full flex-col items-center justify-center gap-3 lg:items-start">
	<h1 class="mb-2 text-center text-4xl font-semibold text-purple-600">Rafael Louie V. Miguel</h1>
	<p class="text-center text-lg text-muted-foreground">
		Bachelor of Science in Information Technology
	</p>
	<p class="text-center text-lg text-muted-foreground">
		Polytechnic University of the Philippines - Manila
	</p>
</div>
<div class="grid gap-6 md:grid-cols-2">
	<Card.Root class="flex items-center justify-center">
		<img src={profilePicture} alt="profile picture" class="h-[250px] w-[250px] rounded-full" />
	</Card.Root>
	<Card.Root class="">
		<Card.Header>
			<Card.Title>Welcome to My E-Portfolio</Card.Title>
			<Card.Description
				>Hello and welcome! I'm excited to share my academic journey and professional growth with
				you through this e-portfolio. Here, you'll find a collection of my projects, achievements,
				and reflections that showcase my skills and experiences in the field of Data Science.</Card.Description
			>
		</Card.Header>
		<Card.Content>
			<p class="text-md mb-2">This portfolio contains:</p>
			<ul class="mb-4 list-inside list-disc space-y-1 text-sm">
				<li>Academic projects and research</li>
				<li>Quizzes</li>
				<li>Assignments</li>
				<li>Exams</li>
			</ul>
			<p class="text-sm">
				Feel free to explore and learn more about my work and aspirations in the world of
				technology!
			</p>
		</Card.Content>
	</Card.Root>
	<Card.Root class="">
		<Card.Header>
			<Card.Title>Midterm Tasks</Card.Title>
		</Card.Header>
		<Card.Content>
			<p class="text-md mb-2">This portfolio contains:</p>
			<ul class="mb-4 list-inside list-disc space-y-1 text-sm">
				<li>Academic projects and research</li>
				<li>Quizzes</li>
				<li>Assignments</li>
				<li>Exams</li>
			</ul>
		</Card.Content>
		<Card.Footer>
			<Button href="/midterm" class="flex w-full items-center gap-2">
				<Telescope class="h-5 w-5" /> View
			</Button>
		</Card.Footer>
	</Card.Root>
	<Card.Root class="">
		<Card.Header>
			<Card.Title>Final Tasks</Card.Title>
		</Card.Header>
		<Card.Content>
			<p class="text-md mb-2">This portfolio contains:</p>
			<ul class="mb-4 list-inside list-disc space-y-1 text-sm">
				<li>Academic projects and research</li>
				<li>Quizzes</li>
				<li>Assignments</li>
				<li>Exams</li>
			</ul>
		</Card.Content>
		<Card.Footer>
			<Button href="/final" class="flex w-full items-center gap-2">
				<Telescope class="h-5 w-5" /> View
			</Button>
		</Card.Footer>
	</Card.Root>
</div>
