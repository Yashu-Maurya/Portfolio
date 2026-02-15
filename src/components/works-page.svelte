<script lang="ts">
	import Work from '../components/work.svelte';

	interface Project {
		project_title: string;
		project_description: string;
		project_link: string;
	}

	let projects: Project[] = [
		{
			project_title: 'CNeuralNet',
			project_description:
				'A lightweight neural network library written in pure C. Provides matrix operations and layer abstractions for building and training simple neural networks from scratch.',
			project_link: 'https://github.com/Yashu-Maurya/CNeuralNet'
		},
		{
			project_title: 'CParticleSimulator',
			project_description:"This project is a collection of 2D physics simulations developed in C using the Raylib library for visualization. It demonstrates various physical phenomenons and also provides abstractions and pre defined structs for making custom simulations.",
			project_link: 'https://github.com/Yashu-Maurya/CParticleSimulator'
		},
	];
</script>

<div class="wrapper">
	<h1 class="title">Selected Works</h1>
	{#each projects as project}
		<Work
			work_title={project.project_title}
			work_description={project.project_description}
			work_link={project.project_link}
		></Work>
	{/each}
</div>

<style>
	.wrapper {
		display: flex;
		flex-direction: column;
		max-width: 1234px;
		padding: 16px;
		margin: auto auto;
		font-family: 'inter';
		font-size: 28px;

        margin-bottom: 64px;

	}

	.title {
		text-align: end;
	}
</style>
