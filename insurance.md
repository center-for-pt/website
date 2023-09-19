---
layout: default
title: Resources
---

<section>
  <h3>Accepted Insurances</h3>

  <p>We accept the following insurances for treatment. Please contact us if you have any questions.</p>

  <ul class="insurance-list">
    {% for insurance in site.data.insurances %}
      {% if insurance.accepted %}
        <li>
          {{ insurance.title }}
        </li>
      {% endif %}
    {% endfor  %}
  </ul>
  <br>
  <p>We <strong>do not</strong> accept the follow insurances.</p>

  <ul class="insurance-list">
    {% for insurance in site.data.insurances %}
      {% unless insurance.accepted %}
        <li>
          {{ insurance.title }}
        </li>
      {% endunless %}
    {% endfor  %}
  </ul>
</section>

