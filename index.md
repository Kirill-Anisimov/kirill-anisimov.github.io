---
layout: default
---
<!-- The main content area -->
<div class="avatarka" style="background-image:url('{{ site.baseurl }}/assets/images/typewriter.jpg'); background-size:cover; position:'center center'; repeat:no-repeat; width:100%; height:250px">
	<a class="header__title" href="{{ '/' | absolute_url }}"></a>
</div>

<div class="posts">
  <div class="grid-xlarge">
    <div class="posts__container" itemscope itemtype="http://schema.org/Blog" data-columns>

      {% for post in paginator.posts %}

        <!-- The tag below includes the markup for each post - partials/post-card.html -->
        {% include post-card.html %}

      {% endfor %}
    </div>
  </div>

  {% include pagination.html %}
</div>