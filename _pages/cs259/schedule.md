---
title: "CS 259 Schedule"
permalink: /cs259/schedule/
---

The week-by-week plan for the course. Dates, slides, and announcements for the current offering are posted in BruinLearn.

<div class="course-table-scroll">
<table class="course-table course-schedule">
  <thead>
    <tr><th>Week</th><th>Topic</th><th>Released</th><th>Milestones</th></tr>
  </thead>
  <tbody>
  {% for w in site.data.courses.cs259 %}
    <tr{% if w.exam %} class="course-exam"{% endif %}>
      <td data-label="Week">{{ w.week }}</td>
      <td data-label="Topic">{{ w.topic }}{% if w.slides %} · <a href="{{ w.slides }}">slides</a>{% endif %}{% if w.note %}<br><small>{{ w.note }}</small>{% endif %}</td>
      <td data-label="Released">{% for item in w.out %}<span class="course-tag">{{ item }}</span>{% endfor %}</td>
      <td data-label="Milestones">{% if w.exam %}<span class="course-tag course-tag--exam">{{ w.exam }}</span> {% endif %}{{ w.milestone }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
</div>

Labs run for two weeks. Paper critiques are due one week after release. See [Assignments]({{ '/cs259/assignments/' | relative_url }}) for details.
