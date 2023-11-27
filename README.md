# CHANGE THESE


"theme.liquid"
"main-product.liquid"
"product-thumbnail.liquid"


## Change currency


## theme.liquid
Add this: 
```
{%- if template.name == 'product' -%}
  <link rel="amphtml" href="{{ shop.url }}/amp/products/{{ product.handle }}">
{%- endif -%}
```
Below:
```
<link rel="canonical" href="{{ canonical_url }}">
```

## Add Default Image
Change media.preview_image to IMG URL

## Add random tagline on title on meta
```
{% assign random_number = "now" | date: "%N" | modulo: 3 %}

{% case random_number %}
  {% when 0 %}
    A
  {% when 1 %}
    B
  {% when 2 %}
    C
{% endcase %}

```


## Add random Tagline on title on Product
```
{% assign random_number = "now" | date: "%N" | modulo: 3 %}

{% case random_number %}
  {% when 0 %}
    A
  {% when 1 %}
    B
  {% when 2 %}
    C
{% endcase %}

```