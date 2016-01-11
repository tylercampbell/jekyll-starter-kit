---
layout: default
---
# AESOP'S FABLES

## A NEW TRANSLATION BY V. S. VERNON JONES

### WITH AN INTRODUCTION BY G. K. CHESTERTON AND ILLUSTRATIONS BY ARTHUR RACKHAM

1912 EDITION

{% for fable in site.fables %}
  <article>
    <a href="{{ fable.url | prepend: site.baseurl }}">{{ fable.title }}</a>
    {% if fable.moral %}{{ fable.moral }}{% endif %}
  </article>
{% endfor %}

![cover](assets/images/cover.jpg)
