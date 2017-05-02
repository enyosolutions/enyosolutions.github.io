# enyosolutions.github.io

It was all a dream
I used to read Word Up magazine
Salt'n'Pepa and Heavy D up in the limousine
Hangin' pictures on my wall
Every Saturday Rap Attack, Mr. Magic, Marley Marl
I let my tape rock 'til my tape pop
Smokin' weed and bamboo, sippin' on private stock
Way back, when I had the red and black lumberjack



<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
