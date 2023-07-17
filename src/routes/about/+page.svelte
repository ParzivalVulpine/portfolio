<script>
	import skills from '$lib/Skills';
</script>

<svelte:head>
	<title>Daniel Gaitan — About</title>
</svelte:head>

<div class="container">
	<main>
		<h1>About</h1>
		<p>
			
			Hey there! I'm Daniel Gaitan, a passionate and award-winning game development student from Drury University. 
			As I approach the end of my senior year, I'm thrilled to dive headfirst into the industry and make a meaningful 
			impact. Throughout my studies, I've been laser-focused on creating captivating game systems and mechanics that 
			truly engage players. What truly excites me is the power of collaboration— I thrive when working with teams, 
			pooling our talents to create something truly extraordinary.
		</p>
		<p>
			I firmly believe that games offer a unique medium for storytelling and experiences that can't be found anywhere 
			else. It's my dream to leverage this power and tell compelling narratives through my creations. When I'm not 
			immersed in game development, you can find me exploring a wide range of video games, carefully dissecting the 
			design decisions that developers have made. I'm always eager to uncover the underlying reasons behind their 
			choices and find ways to improve upon them.
		</p>
		<p>
			I'm eager to embark on this exciting journey and contribute to projects that push the boundaries of interactive 
			entertainment. Let's create something remarkable together!
		</p>
		<h2>Skills</h2>
		{#each Object.entries(skills) as [section, technologies]}
			<ul>
				<li>
					<h4>
						{section}:
					</h4>
					<div class="list">
						{#each technologies as technology}
							<div>
								{technology}
							</div>
						{/each}
					</div>
				</li>
			</ul>
		{/each}
		<h2>Relevant Experience</h2>
		<h3>Drury University - Computer Science Tutor</h3>
		<p>
			<ul>
			<li>Provided individual and group tutoring to help students understand computer science concepts, programming languages, algorithms, and data structures.</li>
			<li>Aided students with assignments, projects, and lab exercises, offering guidance on problem-solving techniques, debugging, and coding best practices.</li>
			<li>Analyzed students' code submissions, identified errors, suggested improvements, and provided constructive feedback to enhance their programming skills.</li>
			<li>Broke down complex computer science concepts into simpler terms, using effective teaching methods and resources to facilitate comprehension.</li>
			</ul>
		<h2>Education</h2>
		<h3>Drury University 
			<br/> Bachelor of Science in Software Engineering - Game Development</h3>
		<p>
			<ul>
			<li>Drury's Indie Game Studio President 2023-2024</li>
			<li>Math & Computer Science Club Vice-President 2023 - 2024</li>
			<li>Relevant coursework: <ul>
			<li>Data Structures</li>
			<li>Application Development I & II</li>
			<li>Foundations of Game Development</li>
			<li>Advanced Game Development</li></ul>
		</ul>
	</main>
</div>

<style>
	.container {
		max-width: 900px;
		padding: 0;
		display: flex;
		justify-content: center;
	}

	main {
		max-width: 100%;
		min-height: 500px;
		text-align: left;
		margin: 0 auto;
		box-sizing: border-box;
	}

	h1 {
		font-weight: 700;
		margin: 0 0 50px 0;
		font-size: 36px;
		text-align: start;
	}

	h2 {
		margin-top: 50px;
	}

	.list {
		display: flex;
		flex-direction: column;
		gap: 30px;
	}

	@media (min-width: 900px) {
		.list {
			flex-direction: row;
		}
		main > h1 {
			font-size: 48px;
		}
	}
</style>
