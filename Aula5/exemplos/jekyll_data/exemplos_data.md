---
layout: default
---

# Esses dados estão em _data/dados.yml

{% for i in site.data.dados.exemplos %}
  - {{ i }}
{% endfor %}

# Outros dados:


{% for i in site.data.dados.outros_exemplos %}
  {% if i.idade < 18 %}
  - {{ i.nome }} (menor)
  {% else %}
  - {{ i.nome }} 
  - {{ i.idade }} 
  {% endif %}
{% endfor %}
