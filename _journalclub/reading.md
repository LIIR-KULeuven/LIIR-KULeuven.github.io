---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Journal-Club @ LIIR - (Past) Reading Papers
permalink: /journal-club/reading/
layout: single
---

Here you can find a list with all the past and upcoming reading club papers.
The presenters are selected from a randomly shuffled queue. Of course it happens that you cannot make it sometimes. 
Just let us know in time so we inform the next person in the queue. The queue of next-up-presenters is
[here]({{"https://docs.google.com/spreadsheets/d/e/2PACX-1vQiFA-Kl6bzHGR33x4Yp1co03fjBH37qe-tfS4fkd0wzRlIW5pMlynJXN-IsuNSxmdv7y2S35hbaK3F/pubhtml" | url}}).

| When&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Who&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | What |    
| --- | --- | --- |  
{%- assign sorted = site.data.reading_sessions | sort: 'date' | reverse -%}
{% for article in sorted %}
| {{ article.date | date_to_string }} {{article.time}} | {{ article.leader }} | 
{%- if article.url == "" -%}
<b> To Be Determined </b>
{%- else -%}
{{ article.description }}  
{%- endif %}<br /> 
{%- if article.url == "" -%}
<b> SEE SLACK FOR POLLY </b>
{%- else -%}
[Link to Paper]({{ article.url | url }}) |  
{%- endif %}
{%- endfor %}
| --- | --- | --- |  

