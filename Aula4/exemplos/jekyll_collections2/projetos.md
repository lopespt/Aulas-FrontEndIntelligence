---
layout: default
---

<h2>Projetos</h2>

<div>
  Essa é uma página que usa uma coleção. A coleção foi definida no arquivo <i>_config.yml</i>.<br/>
  Cada arquivo dentro da pasta <i>_projetos</i> é um item da coleção e pode ser acessado através do atributo <i>site.projetos</i>.
</div>

``` html {% raw %}
<ul>
    {% for projeto in site.projetos %}
    <li>
        {{projeto.content}}
    </li>
    {%endfor %}
</ul> {% endraw %} 
```

<ul>
    {% for projeto in site.projetos %}
    <li>
      Cagegoria: {{ projeto.categoria }}<br/>
        {{projeto.content | markdownify}}
        <a href="{{ projeto.url }}">link</a>
    </li>
    {%endfor %}
</ul>
