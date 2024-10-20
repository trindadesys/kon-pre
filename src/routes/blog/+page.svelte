<script>
	let blogPosts = [
		{
			title: "5 Essential Leadership Skills for 2023",
			excerpt: "Discover the key leadership skills that will drive success in the modern business landscape.",
			date: "2023-05-15",
			category: "Leadership",
			slug: "essential-leadership-skills-2023"
		},
		{
			title: "The Impact of AI on Corporate Training",
			excerpt: "Explore how artificial intelligence is revolutionizing the way companies approach employee training.",
			date: "2023-05-01",
			category: "Training",
			slug: "ai-impact-corporate-training"
		},
		{
			title: "Navigating Change: A Guide for Businesses",
			excerpt: "Learn effective strategies for managing organizational change in uncertain times.",
			date: "2023-04-20",
			category: "Consulting",
			slug: "navigating-change-business-guide"
		}
	];
</script>

<svelte:head>
	<title>Blog - Kon Training e Consulting</title>
	<meta name="description" content="Latest insights, tips, and updates from Kon Training e Consulting" />
</svelte:head>

<div class="blog-page">
	<h1>Our Blog</h1>

	<div class="search-bar">
		<input type="text" placeholder="Search articles..." />
		<button>Search</button>
	</div>

	<div class="blog-grid">
		{#each blogPosts as post}
			<article class="blog-post">
				<h2><a href="/blog/{post.slug}">{post.title}</a></h2>
				<p class="post-meta">
					<span class="date">{post.date}</span>
					<span class="category">{post.category}</span>
				</p>
				<p>{post.excerpt}</p>
				<a href="/blog/{post.slug}" class="read-more">Read More</a>
			</article>
		{/each}
	</div>

	<div class="categories">
		<h3>Categories</h3>
		<ul>
			<li><a href="/blog/category/leadership">Leadership</a></li>
			<li><a href="/blog/category/training">Training</a></li>
			<li><a href="/blog/category/consulting">Consulting</a></li>
			<li><a href="/blog/category/industry-news">Industry News</a></li>
		</ul>
	</div>
</div>

<style>
	.blog-page {
		max-width: 800px;
		margin: 0 auto;
		padding: 2rem 1rem;
	}

	h1 {
		font-size: 2.5rem;
		color: var(--color-theme-1);
		margin-bottom: 2rem;
	}

	.search-bar {
		display: flex;
		margin-bottom: 2rem;
	}

	.search-bar input {
		flex-grow: 1;
		padding: 0.5rem;
		font-size: 1rem;
		border: 1px solid #ccc;
		border-radius: 4px 0 0 4px;
	}

	.search-bar button {
		padding: 0.5rem 1rem;
		font-size: 1rem;
		background-color: var(--color-theme-1);
		color: white;
		border: none;
		border-radius: 0 4px 4px 0;
		cursor: pointer;
	}

	.blog-grid {
		display: grid;
		grid-template-columns: 1fr;
		gap: 2rem;
	}

	.blog-post {
		background-color: #f5f5f5;
		padding: 1.5rem;
		border-radius: 8px;
	}

	.blog-post h2 {
		font-size: 1.5rem;
		margin-bottom: 0.5rem;
	}

	.blog-post h2 a {
		color: var(--color-theme-2);
		text-decoration: none;
	}

	.post-meta {
		font-size: 0.9rem;
		color: #666;
		margin-bottom: 1rem;
	}

	.post-meta .category {
		margin-left: 1rem;
	}

	.read-more {
		display: inline-block;
		margin-top: 1rem;
		color: var(--color-theme-1);
		text-decoration: none;
		font-weight: bold;
	}

	.categories {
		margin-top: 3rem;
	}

	.categories h3 {
		font-size: 1.2rem;
		color: var(--color-theme-2);
		margin-bottom: 1rem;
	}

	.categories ul {
		list-style-type: none;
		padding: 0;
	}

	.categories li {
		margin-bottom: 0.5rem;
	}

	.categories a {
		color: var(--color-text);
		text-decoration: none;
	}

	.categories a:hover {
		color: var(--color-theme-1);
	}
</style>