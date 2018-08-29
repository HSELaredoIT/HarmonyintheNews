---
layout: landing_page
---

<!-- Section -->
<section>
	<header class="major">
		<h2>What is FIRST Robotics Competition?</h2>
	</header>
	<div class="features">
		<article>
			<span class="icon fa-flask"></span>
			<div class="content">
				<h3>Impact</h3>
				<p>The positive impact on FIRST Tech Challenge participants is gratifying and well documented. Over 86% have more interest in doing well in school and 87% are more interested in attending college.</p>
			</div>
		</article>
		<article>
			<span class="icon fa-hand-grab-o"></span>
			<div class="content">
				<h3>Team Basics</h3>
				<p>The really cool thing about FIRST Tech Challenge is being part of a team. All skill levels are welcomed and needed, technical and non-technical. Read on for more about team basics, time frame, commitment, and skills required.</p>
			</div>
		</article>
		<article>
			<span class="icon fa-graduation-cap"></span>
			<div class="content">
				<h3>Scholarships</h3>
				<p>A big advantage to participating in FIRST is gaining access to millions in college scholarships made available by colleges, universities, and corporations who support FIRST. This is exclusive financial help open only to FIRST team members, giving them a competitive leg up on other students seeking educational funds.</p>
			</div>
		</article>
		<article>
			<span class="icon fa-line-chart"></span>
			<div class="content">
				<h3>The Event Experience</h3>
				<p>Hard work pays off! Each FIRST Tech Challenge season culminates with local and regional events where qualifying teams compete for awards and a spot in the FIRST Championship.</p>
			</div>
		</article>
	</div>
</section>


<!-- Section -->
<section>
	<header class="major">
		<h2>Featured Posts</h2>
	</header>
	<div class="posts">



<!--	{% for post in site.posts limit:6 %}
		<article>
			<a href="{{ post.url | relative_url }}" class="image"><img src="{{ '/' | absolute_url }}{{ post.image }}" alt="{{ post.title }}" /></a>
			<h3>{{ post.title }}</h3>
			{{ post.excerpt }}
			<ul class="actions">
				<li><a href="{{ post.url | relative_url }}" class="button">More</a></li>
			</ul>
		</article>
	{% endfor %} -->

		{% for post in site.tags.featured limit: 6 %}
		<article>
			<a href="{{ post.url | relative_url }}" class="image"><img src="{{ '/' | absolute_url }}{{ post.image }}" alt="{{ post.title }}" /></a>
			<h3>{{ post.title }}</h3>
			{{ post.excerpt }}
			<ul class="actions">
				<li><a href="{{ post.url | relative_url }}" class="button">More</a></li>
			</ul>
		</article>
		{% endfor %}

	</div>
</section>
