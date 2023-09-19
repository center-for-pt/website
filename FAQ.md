---
layout: default
title: Resources
---

<section>
  <h3>Patient FAQ</h3>

  <ul>
    {% for faq in site.data.faq %}
    <li>
      <details>
        <summary>
          {{ faq.q }}
        </summary>

        {{ faq.a }}
      </details>
    </li>
    {% endfor %}
  </ul>
</section>