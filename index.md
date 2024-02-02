---
layout: page
title: Home / Lectures
nav_order: 1
description: A description of the content covered in the course.
currWeekNumber: 1
---

{: .mb-2 }
Ferdowsi University of Mashhad, Spring 2023
{: .mb-0 .fs-6 .text-grey-dk-000 }


<div>
{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
  <div class="role">
    {% for staffer in instructors %}
    {{ staffer }}
    {% endfor %}
  </div>
</div>

{: .highlight }
> Welcome to the Course!


<a name="lectures"></a>
## Lectures

{% for module in site.modules %}
{{ module }}
{% endfor %}

