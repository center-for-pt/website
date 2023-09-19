---
layout: default
title: Resources
---

<section>
  <h3>Patient Forms</h3>

  <p>The following forms are available as downloadable documents. Please print those that apply to you, fill them out and bring them to your initial evaluation.</p>

  <ul>
    {% for patient_form in site.data.patient_forms %}
      <li>
        <a href="{{ patient_form.url }}" target="_blank">
          {{ patient_form.title }}
        </a>
      </li>
    {% endfor %}
  </ul>
</section>
