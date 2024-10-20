<script>
	import welcome from '$lib/images/welcome-image.jpg';
</script>

<svelte:head>
	<title>Kon Training e Consulting</title>
	<meta name="description" content="Professional training and consulting services" />
</svelte:head>

<section class="hero">
	<img src={welcome} alt="Welcome to Kon Training e Consulting" />
	<div class="hero-content">
		<h1>Empowering Your Business Through Expert Training and Consulting</h1>
		<p>Unlock your team's potential with our tailored solutions</p>
		<a href="/contact" class="cta-button">Get Started</a>
	</div>
</section>

<section class="services">
	<h2>Our Services</h2>
	<div class="service-grid">
		<div class="service-item">
			<h3>Corporate Training</h3>
			<p>Enhance your team's skills with our customized training programs.</p>
		</div>
		<div class="service-item">
			<h3>Business Consulting</h3>
			<p>Strategic advice to help your business grow and succeed.</p>
		</div>
		<div class="service-item">
			<h3>Leadership Development</h3>
			<p>Nurture the next generation of leaders in your organization.</p>
		</div>
	</div>
	<a href="/services" class="learn-more">Learn More About Our Services</a>
</section>

<section class="testimonials">
	<h2>What Our Clients Say</h2>
	<div class="testimonial-grid">
		<blockquote>
			"Kon Training transformed our team's productivity. Highly recommended!"
			<footer>- John Doe, CEO of TechCorp</footer>
		</blockquote>
		<blockquote>
			"The consulting services provided invaluable insights for our business strategy."
			<footer>- Jane Smith, Director at InnovateCo</footer>
		</blockquote>
	</div>
</section>

<style>
	.hero {
		position: relative;
		height: 400px;
		overflow: hidden;
	}

	.hero img {
		width: 100%;
		height: 100%;
		object-fit: cover;
	}

	.hero-content {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		text-align: center;
		color: white;
		background-color: rgba(0, 0, 0, 0.5);
		padding: 2rem;
		border-radius: 8px;
	}

	.hero h1 {
		font-size: 2.5rem;
		margin-bottom: 1rem;
	}

	.cta-button {
		display: inline-block;
		background-color: var(--color-theme-1);
		color: white;
		padding: 0.5rem 1rem;
		border-radius: 4px;
		text-decoration: none;
		font-weight: bold;
		margin-top: 1rem;
	}

	.services, .testimonials {
		padding: 2rem 0;
	}

	.service-grid, .testimonial-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
		gap: 2rem;
		margin-top: 2rem;
	}

	.service-item {
		background-color: #f5f5f5;
		padding: 1.5rem;
		border-radius: 8px;
		text-align: center;
	}

	.learn-more {
		display: block;
		text-align: center;
		margin-top: 2rem;
		color: var(--color-theme-1);
		text-decoration: none;
		font-weight: bold;
	}

	blockquote {
		background-color: #f5f5f5;
		padding: 1.5rem;
		border-radius: 8px;
		font-style: italic;
	}

	blockquote footer {
		margin-top: 1rem;
		font-style: normal;
		font-weight: bold;
	}
</style>