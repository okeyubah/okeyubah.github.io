{% if page.title %}
      {{ page.title }}
      {% else %}
   {{ No page title here! }}
    {% endif %}
    
    {% if user %}
      Hello {{ user.name }}!
    {% endif %}
    
    {{ "/my/fancy/url" | append: ".html" }}
    {{"adam!" | capitalize | prepend: "Hello" }}

 {% for product in site.data.products %}{% if product.title == "Awesome Shoes" %}
      Those shoes are awesome.
    {% endif %}
    {% endfor %}
    
{% for product in site.data.products %}
  {% if product.type == "Shoes" or product.type == "Shirt" %}
    This is a shirt or a pair of shoes. Name: {{ product.name }}
  {% endif %}
{% endfor %}   

 {% for product in site.data.products %}
  {% if product.name contains "Systems" %}
    Product name contains System. Name: {{ product.name }}
  {% endif %}
{% endfor %} 

{% assign my_string = "Hello World!" %}
    {% assign my_int = 25 %}
    {% assign my_float = 23.756 %}
    {{ my_string }}
    {{ my_int }}
    {{ my_float }}
    
    {% assign foo = true %}
    {% assign bar = false %}
    {{ foo }}
    {{ bar }}
    
 {% assign users = "Chidi, Nwafor, Tunde, Balarabe, Etim" | split: ", " %}
    {% for user in users %}
      {{ user }}
    {% endfor %}
    
