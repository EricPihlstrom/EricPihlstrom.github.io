---
layout: default
title: "Weekly Project Updates"
description: CSPB 3112
permalink: /weeklyUpdates
---

<div class="container">
    {% for week in site.data.weekly_updates %}
    <h2>{{ week.title }}</h2>
    <h4>What did you do last week?</h4>
    <ul>
        {% for item in week.last_week %}
        <li>{{ item }}</li>
        {% endfor %}
    </ul>
    <h4>What do you plan to do this week?</h4>
    <ul>
        {% for item in week.this_week %}
        <li>{{ item }}</li>
        {% endfor %}
    </ul>
    <h4>Are there any impediments in your way?</h4>
    <ul>
        {% for item in week.impediments %}
        <li>{{ item }}</li>
        {% endfor %}
    </ul>
    <h4>Reflection on the process you used last week, how can you make the process work better?</h4>
    <ul>
        {% for item in week.reflection %}
        <li>{{ item }}</li>
        {% endfor %}
    </ul>
    {% endfor %}
</div>
