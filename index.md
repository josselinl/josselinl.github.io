---
layout: home  # ou "default" si pas de home layout
title: "Blog PKI Josselin L."
paginate: 5   # 5 posts par page (optionnel)
---

# Derniers articles PKI

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="date">{{ post.date | date: "%d/%m/%Y" }}</p>
    <div class="excerpt">{{ post.excerpt | strip_html }}</div>  <!-- Résumé auto -->
    <a href="{{ post.url }}">Lire la suite →</a>
  </article>
{% endfor %}

{% if paginator.total_pages > 1 %}
  <div class="pagination">
    {% if paginator.previous_page %}
      <a href="/page{{ paginator.previous_page }}">← Précédent</a>
    {% endif %}
    Page {{ paginator.page }} sur {{ paginator.total_pages }}
    {% if paginator.next_page %}
      <a href="/page{{ paginator.next_page }}">Suivant →</a>
    {% endif %}
  </div>
{% endif %}
