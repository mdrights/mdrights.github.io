---
layout: page
title: Autonomy on Medicine
permalink: /autonomy/
---

<div class="tag-page">
	
	<p class="post-meta">
		{{ site.tags[page.title] | size }} 篇文章
	</p>
	
	<ul class="post-list">
		{% for post in site.tags[page.title] %}
		<li>
			
			<h2>
				<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
			</h2>
		</li>
		{% endfor %}
	</ul>
	
</div>
