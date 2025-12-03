/_blog
 /tech
  /ai
   post1.md
   post2.md
 /web
   post3.md
/lifestyle
 /travel
 post4

 layout🏤
 title: "Understanding AI Agents"
 permalink: /blog/tech/ai/understand:

 layout: default
 title: Blog
 permalink: /blog/

 [Tech](/blog/tech/)
 [Lifestyle](/blog/lifestyle/)

 layout: default
 title: Tech
 permalink: /blog/tech/

 [AI](/blog/tech/ai/)
 [Web](/blog/tech/web/)

 collections:
   tech_ai
     output: true
     permalink: /blog/tech/ai/📛
  tech_web:
    output: true
    permalink: /blog/tech/web/📛

    layout: default
    title: AI Posts
    permalink: /blog/tech/ai/

    {% for page in site.pages %}
     {% if page.url contains '/blog/tech/ai/' andpage.title # 'AI Posts' %}
     - [{{ page.title}}]({{ page.url }})
     {% endif %}
   {% endfor %}

   collections:
     tech_ai
       output: true
       permalink: /blog/tech/ai/:name/
    lifestyle_travel:
       output: true
       permalink: /blog/lifestyle/travel/:name/

    {% for page in site.pages %}
     {% if page.url contains '/blog/lifestyle/travel/' %}
     - [{{ page.title}}]({{page.url }})
     {% endif %}
  {% endfor %}
  
       
       
