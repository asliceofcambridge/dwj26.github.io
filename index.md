---
layout: default
title: A Slice of Cambridge
---

[![image-title-here](/assets/img/logo.png){:class="img-responsive"}{:id="title-banner"}](/about/)

<p></p>
<h3 align = "center" class = "homeh3"><span>Featured</span></h3>
<div class="container">
    <div class="row">
            {% for post in site.posts %}
            {% if post.featured %}
                <div class="col-md-12 col-xl-4">
									  <a href="{{ post.url }}">
												<div class="grid-banner" style="background-image: url('{{ post.featured-img }}');">
													<div class = "middle">
													<h3>{{ post.title }}</h3>
													<p>{{post.date | date_to_string}}</p>
												</div>
												<p></p>
											</div>
										</a>
                </div>
              {% endif %}
            {% endfor %}

    </div>

</div>


<p></p>
<h3 align = "center" class = "homeh3"><span>All Posts</span></h3>
<div class="container">
    <div class="row">
            {% for post in site.posts %}
                <div class="col-md-12 col-xl-4">
									  <a href="{{ post.url }}">
												<div class="grid-banner" style="background-image: url('{{ post.featured-img }}');">
													<div class = "middle">
													<h3>{{ post.title }}</h3>
													<p>{{post.date | date_to_string}}</p>
												</div>
												<p></p>
											</div>
										</a>

                </div>
            {% endfor %}

    </div>

</div>
