---
layout: page
permalink: /teaching/
title: Teaching
description: 
nav: true
nav_order: 5
calendar: true
---

<!-- This page displays a collection of courses with detailed schedules, materials, and resources. You can organize your courses by years, terms, or topics.

{% include calendar.liquid calendar_id='test@gmail.com' timezone='Asia/Shanghai' %}

{% include courses.liquid %} -->

<!-- ### CPT208 Human-Centric Computing -->


<!-- ### CPT411 Evaluation Methods and Statistics -->

I am happy to supervise **final year projects** in SAT301, SAT405 and SAT406, as well as **summer research** for HCI/VR/AR related projects. For students who are interested in doing projects with me, please feel free to send me an email: yue.li@xjtlu.edu.cn. Highly motivated students with skills or experience in VR development (Unity), 3D modeling, and AIGC are very welcomed.

<div style="margin-bottom:2.5rem">
</div>

### Student Competitions and Awards

<div style="margin-bottom:2.5rem">
  {% include students_competitions.liquid %}
</div>

### Taught Students (FYPs and FMPs)
<style>
.teaching-grid {
  column-count: auto;
  columns: 280px;
  column-gap: 1.5rem;
  column-fill: balance;
  margin: 2rem 0;
}

.teaching-card {
  background: var(--global-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 8px;
  padding: 1.25rem;
  transition: all 0.3s ease;
  margin-bottom: 1.5rem;
  break-inside: avoid;
  page-break-inside: avoid;
}

.teaching-card:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  transform: translateY(-2px);
}

.teaching-card h3 {
  margin: 0 0 0.75rem 0;
  font-size: 1rem;
  font-weight: 600;
  color: var(--global-text-color);
}

.teaching-card .students {
  font-size: 0.9rem;
  line-height: 1.5;
  color: var(--global-text-color);
  opacity: 0.85;
}

.teaching-card .student-item {
  display: flex;
  justify-content: space-between;
  margin-bottom: 0.25rem;
}

.teaching-card .student-name {
  flex: 1;
  word-break: break-word;
}

.teaching-card .grad-year {
  flex-shrink: 0;
  margin-left: 0.5rem;
  color: var(--global-theme-color);
  font-weight: 500;
}

.research-students-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 1.5rem;
  row-gap: 1.5rem;
  margin: 2rem 0;
}

@media (max-width: 1200px) {
  .research-students-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 768px) {
  .research-students-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="teaching-grid">
  {% for program in site.data.students_fyp %}
    {% include students_fyp_card.liquid program=program %}
  {% endfor %}
</div>
 
### Research Students

<div class="research-students-grid">
  {% for group in site.data.students_research %}
    {% include students_research_card.liquid group=group %}
  {% endfor %}
</div>

