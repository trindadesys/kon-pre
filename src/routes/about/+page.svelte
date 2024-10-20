<svelte:head>
	<title>About Us - Kon Training e Consulting</title>
	<meta name="description" content="Learn about Kon Training e Consulting's history, mission, and team" />
</svelte:head>

<div class="about-page">
	<h1>About Kon Training e Consulting</h1>

	<section class="company-history">
		<h2>Our History</h2>
		<p>Founded in 2010, Kon Training e Consulting has been at the forefront of professional development and business strategy for over a decade. Our journey began with a vision to transform how businesses approach training and consulting services.</p>
	</section>

	<section class="mission-vision">
		<h2>Our Mission & Vision</h2>
		<p><strong>Mission:</strong> To empower businesses and individuals through innovative training and strategic consulting, fostering growth and excellence in every client we serve.</p>
		<p><strong>Vision:</strong> To be the global leader in transformative training and consulting services, known for our commitment to client success and cutting-edge methodologies.</p>
	</section>

	<section class="team-profiles">
		<h2>Our Team</h2>
		<div class="team-grid">
			<div class="team-member">
				<img src="/images/team-member-1.jpg" alt="Jane Doe" />
				<h3>Jane Doe</h3>
				<p>Founder & CEO</p>
			</div>
			<div class="team-member">
				<img src="/images/team-member-2.jpg" alt="John Smith" />
				<h3>John Smith</h3>
				<p>Head of Training</p>
			</div>
			<!-- Add more team members as needed -->
		</div>
	</section>

	<section class="partners">
		<h2>Our Partners & Collaborations</h2>
		<p>We're proud to work with leading organizations across various industries. Our partnerships enable us to provide cutting-edge solutions and stay at the forefront of industry trends.</p>
		<div class="partner-logos">
			<!-- Add partner logos here -->
		</div>
	</section>
</div>

<style>
	.about-page {
		max-width: 800px;
		margin: 0 auto;
		padding: 2rem 1rem;
	}

	h1 {
		font-size: 2.5rem;
		color: var(--color-theme-1);
		margin-bottom: 2rem;
	}

	h2 {
		font-size: 1.8rem;
		color: var(--color-theme-2);
		margin-top: 2rem;
		margin-bottom: 1rem;
	}

	section {
		margin-bottom: 3rem;
	}

	.team-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		gap: 2rem;
		margin-top: 2rem;
	}

	.team-member {
		text-align: center;
	}

	.team-member img {
		width: 150px;
		height: 150px;
		border-radius: 50%;
		object-fit: cover;
		margin-bottom: 1rem;
	}

	.partner-logos {
		display: flex;
		justify-content: space-around;
		align-items: center;
		flex-wrap: wrap;
		margin-top: 2rem;
	}

	.partner-logos img {
		max-width: 150px;
		height: auto;
		margin: 1rem;
	}
</style>