---
layout: default
title: Team
---

<!-- <section>
  <h2>
    Get to know our talented physical therapists!
  </h2>

  <div>
    {% for staff_member in site.staff_members %}
      <div>
        <h3>
          <a href="{{ staff_member.url }}">
            {{ staff_member.name }}
          </a>
        </h3>
        <img alt="{{ staff_member.name }}" src="/assets/images/staff_members/{{ staff_member.slug }}-small.jpg" />
        <p>{{ staff_member.qualifications }}</p>
      </div>
    {% endfor %}
  </div>
</section> -->

<section>
  <h2>
    Meet our physical therapists
  </h2>

  <div id="bio-container" class="content-section">
    <div class="bio-wrapper w-container">
      {% for staff_member in site.staff_members %}
        <div class="bio-card">
          <img class="bio-thumb" alt="{{ staff_member.name }}" src="/assets/images/staff_members/{{ staff_member.slug }}-small.jpg" />
          <h3>
            <a href="{{ staff_member.url }}">
              {{ staff_member.name }}
            </a>
          </h3>
          <p>{{ staff_member.qualifications }}</p>
        </div>
      {% endfor %}
    </div>
  </div>

</section>


