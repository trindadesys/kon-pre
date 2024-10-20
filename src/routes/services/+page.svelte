<svelte:head>
	<title>Our Services - Kon Training e Consulting</title>
	<meta name="description" content="Explore our range of training and consulting services" />
</svelte:head>

<div class="services-page">
	<h1>Our Services</h1>

	<section class="service">
		<h2>Corporate Training</h2>
		<p>Our corporate training programs are designed to enhance your team's skills and boost productivity. We offer customized training solutions in areas such as:</p>
		<ul>
			<li>Leadership Development</li>
			<li>Communication Skills</li>
			<li>Project Management</li>
			<li>Team Building</li>
		</ul>
		<a href="/contact" class="cta-button">Request a Quote</a>
	</section>

	<section class="service">
		<h2>Business Consulting</h2>
		<p>Our expert consultants provide strategic advice to help your business grow and succeed. Our consulting services include:</p>
		<ul>
			<li>Strategic Planning</li>
			<li>Process Optimization</li>
			<li>Change Management</li>
			<li>Market Analysis</li>
		</ul>
		<a href="/contact" class="cta-button">Schedule a Consultation</a>
	</section>

	<section class="service">
		<h2>Leadership Development</h2>
		<p>Nurture the next generation of leaders in your organization with our comprehensive leadership development programs. We focus on:</p>
		<ul>
			<li>Executive Coaching</li>
			<li>Succession Planning</li>
			<li>High-Potential Employee Development</li>
			<li>Leadership Skills Workshops</li>
		</ul>
		<a href="/contact" class="cta-button">Learn More</a>
	</section>

	<section class="case-studies">
		<h2>Case Studies</h2>
		<div class="case-study">
			<h3>TechCorp Productivity Boost</h3>
			<p>Learn how our training program increased TechCorp's team productivity by 35% in just 6 months.</p>
			<a href="/case-studies/techcorp">Read More</a>
		</div>
		<div class="case-study">
			<h3>InnovateCo's Market Expansion</h3>
			<p>Discover how our consulting services helped InnovateCo successfully enter three new markets.</p>
			<a href="/case-studies/innovateco">Read More</a>
		</div>
	</section>
</div>

<style>
	.services-page {
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

	.service {
		margin-bottom: 3rem;
		padding: 2rem;
		background-color: #f5f5f5;
		border-radius: 8px;
	}

	ul {
		margin-left: 1.5rem;
		margin-bottom: 1.5rem;
	}

	.cta-button {
		display: inline-block;
		background-color: var(--color-theme-1);
		color: white;
		padding: 0.5rem 1rem;
		border-radius: 4px;
		text-decoration: none;
		font-weight: bold;
	}

	.case-studies {
		margin-top: 3rem;
	}

	.case-study {
		margin-bottom: 2rem;
		padding: 1.5rem;
		background-color: #f5f5f5;
		border-radius: 8px;
	}

	.case-study h3 {
		color: var(--color-theme-1);
		margin-bottom: 0.5rem;
	}

	.case-study a {
		display: inline-block;
		margin-top: 1rem;
		color: var(--color-theme-1);
		text-decoration: none;
		font-weight: bold;
	}
</style>