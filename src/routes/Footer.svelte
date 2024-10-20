<script>
	import { base } from '$app/paths';
</script>

<footer>
	<div class="footer-content">
		<div class="footer-section">
			<h3>Quick Links</h3>
			<ul>
				<li><a href="{base}/">Home</a></li>
				<li><a href="{base}/about">About Us</a></li>
				<li><a href="{base}/services">Services</a></li>
				<li><a href="{base}/blog">Blog</a></li>
				<li><a href="{base}/contact">Contact</a></li>
			</ul>
		</div>
		<div class="footer-section">
			<h3>Contact Us</h3>
			<p>123 Business Street, City, Country</p>
			<p>Phone: +1 234 567 890</p>
			<p>Email: info@kontraining.com</p>
		</div>
		<div class="footer-section">
			<h3>Follow Us</h3>
			<div class="social-links">
				<a href="#" target="_blank" rel="noopener noreferrer">Facebook</a>
				<a href="#" target="_blank" rel="noopener noreferrer">Twitter</a>
				<a href="#" target="_blank" rel="noopener noreferrer">LinkedIn</a>
			</div>
		</div>
	</div>
	<div class="footer-bottom">
		<p>&copy; 2023 Kon Training e Consulting. All rights reserved.</p>
	</div>
</footer>

<style>
	footer {
		background-color: #f5f5f5;
		padding: 2rem 1rem;
		margin-top: 2rem;
	}

	.footer-content {
		display: flex;
		justify-content: space-between;
		max-width: 64rem;
		margin: 0 auto;
	}

	.footer-section {
		flex: 1;
		margin-right: 2rem;
	}

	.footer-section:last-child {
		margin-right: 0;
	}

	h3 {
		font-size: 1.2rem;
		margin-bottom: 1rem;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	li {
		margin-bottom: 0.5rem;
	}

	a {
		color: var(--color-text);
		text-decoration: none;
	}

	a:hover {
		color: var(--color-theme-1);
	}

	.social-links {
		display: flex;
		gap: 1rem;
	}

	.footer-bottom {
		text-align: center;
		margin-top: 2rem;
		padding-top: 1rem;
		border-top: 1px solid #ddd;
	}
</style>