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
    
    {{ users[0] }}
    {{ users[1] }}
    {{ users[-1] }}
    {{ users[-2] }}   
    
 {% assign name = "ikenna" %}
    {% if name == "uju" %}
      Hello uju
    {% elsif name == "ikenna" %}
      Hello ikenna
    {% else %}
      Hello Stranger
    {% endif %}

{% assign handle = "cake" %}
{% case handle %}
{% when "cake" %}
  This is a cake
{% when "cookie", "biscuit" %}
  This is a cookie
{% else %}
  This is neither a cake, nor a cookie
{% endcase %}

{% for i in (1..5) %}
      {% if i == 4 %}
        {% break %}
      {% else %}
        {{ i }}
      {% endif %}
      {% endfor %}
      
{% for i in (1..5) %}
      {% if i == 4 %}
        {% continue %}
      {% else %}
        {{ i }}
      {% endif %}
      {% endfor %}

{% capture my_variable %}
    I am the value of my_variable
    {% endcapture %}
    <p>{{ my_variable }}</p>

 {% for product in site.data.products %}
    <p>Name: {{ product.name }} Title: {{ product.title}}</p>
    {% if forloop.last == true %}
    This is the last iteration in the forloop
    {% endif %}
{% endfor %}   

{% assign my_var = 'the value' %}
{{ my_var }}

{% assign cheeses = "cheddar, swiss, gouda, havarti, string" | split: ',' %}
<ul>
{% for cheese in cheeses %}
      <li>
        I like {{cheese }}
      </li>
      {% endfor %}
</ul>

{% capture products_list %}
{% for product in site.data.products %}
{{ product.name }} | {{ product.title }} | {{product.location }}
{% if forloop.last == false %}::{% endif %}{% endfor %}{% endcapture %}
{% assign products_array = products_list | split: '::' %}

{% capture products_list %}
{% for product in site.data.products %}
{{ product.name }} | {{ product.title }} | {{product.location }}
{% if forloop.last == false %}::{% endif %}{% endfor %}{% endcapture %}
{% assign products_array = products_list | split: '::' %}
    {% for product in products_array %}
      {% assign product_vals = product | split: '|' %}
      {{ product_vals[0] }}
      {{ product_vals[1] }}    
    {% endfor %}
    
 {% capture person %}
    name: John Doe, age: 20
    {% endcapture %}
    {% assign person = person | split: ', ' %}
    {{ person.first }}
     
  {% assign arrayOne = 'a,b,c' | split: ',' %}
   {% assign arrayTwo = 'd,e,f' | split: ',' %}   
   {% assign foo = arrayOne | concat: arrayTwo %}
   {% for item in foo %}
     {{ item }} 
    {% endfor %}
    
    {{"March 14 2016" | time: "%b %d, %y"}}
    
      This page was last updated on {{ "now" | date: "%d-%m-%Y %H:%M" }}.
    
     Number of pages on this website: {{ site.pages.size }}
