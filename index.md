---
title: Rodolfo Schiavi - Blog
layout: default
---

Welcome to my blog! Here, I share my knowledge and experiences in the world of technology, focusing on backend development, infrastructure, and cybersecurity. Expect to find tutorials, tips, and insights on building robust APIs, managing databases, deploying applications, securing your code, and much more. Stay tuned for engaging and informative content that will help you navigate the tech landscape. Thank you for visiting, and happy coding!

<section class="list">
	{% if site.posts.size == 0 %}
		<p class="text-center">Nothing published yet!</p>
	{% else %}
		{% for post in site.posts %}
				{% if post.hidden != true %}
					{% include blog-post.html %}
				{% endif %}
		{% endfor %}
	{% endif %}
</section>
