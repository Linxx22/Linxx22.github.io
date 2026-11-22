---
permalink: /
---

{% assign email = site.author.links | where: "title", "Email" | first %}

Welcome to my homepage! I am Xuxuan Lin, originally from Anxi, Fujian—a region renowned as a hometown of Chinese tea. I am currently a Ph.D. student in the Department of Electronic Engineering at Tsinghua University, advised by Associate Professor [Yue Li](https://oa.ee.tsinghua.edu.cn/~liyue/), where I also earned my bachelor's degree.

My research began with antenna theory and terminal applications. Alongside my ongoing work on antennas, I actively explore intriguing electromagnetic phenomena and the interdisciplinary connections between electromagnetics and other fields, aiming to bring fresh insights to academia and the broader research community.

Feel free to reach out via [email]({{ email.url }}) for academic discussions or potential collaborations!

# <span aria-hidden="true">🎓</span> Education
{: #education }

{% for school in site.data.education %}
<div class="education-entry">
  <img src="{{ school.logo }}" alt="" width="54" height="54">
  <div>
    <h2>{{ school.institution }}</h2>
    <p class="entry-date">{{ school.period }}</p>
    <p>{{ school.degree }}{% if school.department %}<br>{{ school.department }}{% endif %}</p>
  </div>
</div>
{% endfor %}

# <span aria-hidden="true">📚</span> Publications
{: #publications }

{% include publications.html limit=5 format="text" %}

[All publications →](publications.html)

# <span aria-hidden="true">🏆</span> Awards
{: #awards }

<ul class="award-list">
{% for award in site.data.awards %}
  <li><span class="entry-date">{{ award.date }}</span><div>{{ award.name }}{% if award.note %}<br><small>{{ award.note }}</small>{% endif %}</div></li>
{% endfor %}
</ul>

# <span aria-hidden="true">💼</span> INTERNSHIPS
{: #internships }

{% for internship in site.data.internships %}
<div class="internship-entry">
  {% if internship.logo %}<img src="{{ internship.logo }}" alt="" width="54" height="54">{% endif %}
  <div>
    <h2>{{ internship.company }}</h2>
    <p class="entry-date">{{ internship.period }}</p>
    <p>{{ internship.role }}<br>{{ internship.department }}</p>
  </div>
</div>
{% endfor %}
