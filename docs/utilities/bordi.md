---
layout: docs
title: Bordi
description: Modifica lo stile di bordi e il loro arrotondamento.
group: utilities
redirect_from: "/docs/utilities/"
toc: true
---

Aggiungi o rimuovi il bordo a un elemento. Puoi scegliere fra un bordo completo oppure un lato alla volta, secondo una
logica aggiuntiva o sottrattiva.

### Aggiuntivo

<div class="bd-example-border-utils">
{% example html %}
<span class="border"></span>
<span class="border-top"></span>
<span class="border-right"></span>
<span class="border-bottom"></span>
<span class="border-left"></span>
{% endexample %}
</div>

### Sottrattivo

<div class="bd-example-border-utils bd-example-border-utils-0">
{% example html %}
<span class="border-0"></span>
<span class="border-top-0"></span>
<span class="border-right-0"></span>
<span class="border-bottom-0"></span>
<span class="border-left-0"></span>
{% endexample %}
</div>

## Colore dei bordi

Cambia il colore del bordo usando la palette del tema in uso.

<div class="bd-example-border-utils">
{% example html %}
{% for color in site.data.theme-colors %}
<span class="border border-{{ color.name }}"></span>{% endfor %}
<span class="border border-white"></span>
{% endexample %}
</div>

## Bordi arrotondati

Tutte le classi per arrotondare facilmente gli angoli di un elemento.

<div class="bd-example bd-example-images">
  <img data-src="holder.js/75x75" class="rounded" alt="Esempio di immagine arrotondata">
  <img data-src="holder.js/75x75" class="rounded-top" alt="Esempio di immagine arrotondata in alto">
  <img data-src="holder.js/75x75" class="rounded-right" alt="Esempio di immagine arrotondata a destra">
  <img data-src="holder.js/75x75" class="rounded-bottom" alt="Esempio di immagine arrotondata in basso">
  <img data-src="holder.js/75x75" class="rounded-left" alt="Esempio di immagine arrotondata a sinistra">
  <img data-src="holder.js/75x75" class="rounded-circle" alt="Esempio di immagine arrotondata a cerchio">
  <img data-src="holder.js/75x75" class="rounded-0" alt="Esempio di immagine non arrotondata (sovrascrive l'eventuale arrotondamento applicato precedentemente)">
</div>

{% highlight html %}
<img src="..." alt="..." class="rounded">
<img src="..." alt="..." class="rounded-top">
<img src="..." alt="..." class="rounded-right">
<img src="..." alt="..." class="rounded-bottom">
<img src="..." alt="..." class="rounded-left">
<img src="..." alt="..." class="rounded-circle">
<img src="..." alt="..." class="rounded-0">
{% endhighlight %}
