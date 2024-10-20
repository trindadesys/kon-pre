<script>
	let name = '';
	let email = '';
	let message = '';

	function handleSubmit() {
		// Here you would typically send the form data to a server
		console.log('Form submitted', { name, email, message });
		alert('Thank you for your message. We will get back to you soon!');
		name = '';
		email = '';
		message = '';
	}
</script>

<svelte:head>
	<title>Contact Us - Kon Training e Consulting</title>
	<meta name="description" content="Get in touch with Kon Training e Consulting for your training and consulting needs" />
</svelte:head>

<div class="contact-page">
	<h1>Contact Us</h1>

	<div class="contact-content">
		<div class="contact-form">
			<h2>Send us a message</h2>
			<form on:submit|preventDefault={handleSubmit}>
				<div class="form-group">
					<label for="name">Name</label>
					<input type="text" id="name" bind:value={name} required />
				</div>
				<div class="form-group">
					<label for="email">Email</label>
					<input type="email" id="email" bind:value={email} required />
				</div>
				<div class="form-group">
					<label for="message">Message</label>
					<textarea id="message" bind:value={message} required></textarea>
				</div>
				<button type="submit" class="submit-button">Send Message</button>
			</form>
		</div>

		<div class="contact-info">
			<h2>Contact Information</h2>
			<p><strong>Address:</strong> 123 Business Street, City, Country</p>
			<p><strong>Phone:</strong> +1 234 567 890</p>
			<p><strong>Email:</strong> info@kontraining.com</p>
			<p><strong>Business Hours:</strong> Monday - Friday, 9am - 5pm</p>

			<div class="map">
				<!-- Replace with an actual Google Maps embed -->
				<img src="/images/map-placeholder.jpg" alt="Our Location" />
			</div>
		</div>
	</div>
</div>

<style>
	.contact-page {
		max-width: 1000px;
		margin: 0 auto;
		padding: 2rem 1rem;
	}

	h1 {
		font-size: 2.5rem;
		color: var(--color-theme-1);
		margin-bottom: 2rem;
	}

	.contact-content {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 2rem;
	}

	@media (max-width: 768px) {
		.contact-content {
			grid-template-columns: 1fr;
		}
	}

	h2 {
		font-size: 1.8rem;
		color: var(--color-theme-2);
		margin-bottom: 1rem;
	}

	.form-group {
		margin-bottom: 1rem;
	}

	label {
		display: block;
		margin-bottom: 0.5rem;
	}

	input, textarea {
		width: 100%;
		padding: 0.5rem;
		font-size: 1rem;
		border: 1px solid #ccc;
		border-radius: 4px;
	}

	textarea {
		height: 150px;
	}

	.submit-button {
		background-color: var(--color-theme-1);
		color: white;
		padding: 0.5rem 1rem;
		font-size: 1rem;
		border: none;
		border-radius: 4px;
		cursor: pointer;
	}

	.submit-button:hover {
		background-color: var(--color-theme-2);
	}

	.contact-info p {
		margin-bottom: 0.5rem;
	}

	.map {
		margin-top: 1rem;
	}

	.map img {
		width: 100%;
		height: auto;
		border-radius: 4px;
	}
</style>