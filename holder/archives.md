{% if page.title %}
      {{ page.title }}
      {% else %}
   {{ No page title here! }}
    {% endif %}
    
    {% if user %}
      Hello {{ user.name }}!
    {% endif %}
