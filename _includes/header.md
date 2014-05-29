<header class="inner">
  <nav>
    <a class="{% if page.category == 'home' %} selected {% endif %}" href="/">Home</a>
    <a class="{% if page.category == 'about' %} selected {% endif %}" href="/about">About</a>
    <!--<a class="{% if page.category == 'portfolio' %} selected {% endif %}" href="/portfolio/">Portfolio</a>-->
    <!--<a class="{% if page.category == 'contact' %} selected {% endif %} contact" href="/contact/">Contact</a>-->
    <a class="{% if page.category == 'archive' %} selected {% endif %}" href="/archive/">Archive</a>
    <a class="{% if page.category == 'tag' %} selected {% endif %}" href="/tag/">Tag</a>
    <!--<a href="https://github.com/ssaunier">Github</a>-->
  </nav>
  <div class="pull-right right logo">
    <div class="name">
      <a href="/">{{ site.author.name }}'s Blog</a>
      <a href="/feed.xml" title="Subscribe to my blog with RSS"><i class="icon-feed"></i></a>
      <br />
      <small>
        <em>
          <a href="/">{{ site.description }}</a>
        </em>
      </small>
    </div>
    <!--<img class="avatar" src="/images/seonho_oh.png" alt="My profile picture" />-->
  </div>
  <div class="clear"></div>
</header>
<div class="clear"></div>
