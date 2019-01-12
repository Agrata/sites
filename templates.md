---
layout: default
title:  "Templates"
excerpt:  Choose from a collection of premium HTML5 templates, built by creators around the world.
---

<div class="section text-center section-examples">
      <div class="row">
            <div class="col-md-8 ml-auto mr-auto">
                  <h2 class="title">Themes</h2>
                  <h5 class="description">A collection of simple HTML5 & WordPress templates, built by creators around the world.</h5>
            </div>
	</div>
	<br>
      <div class="container-fluid text-center">
        <div class="row">
	<ul>
          {% for post in site.posts %}
		<li>
		<div class="col-md-6">
			<a href="{{ post.url }}" title="{{ post.title }}">
              		<img src="{{ post.img }}" class="img-raised rounded img-fluid">
              		<button class="btn  btn-link btn-primary btn-lg">{{ post.title }}</button>
            		</a>
          	</div>
		</li>
          {% endfor %}
	  </ul>
        </div>
      </div>
</div>
