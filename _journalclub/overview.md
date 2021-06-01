---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: LIIR \| Journal-Club
permalink: /journal-club/
---
![jc-logo]({{site.url}}{{site.baseurl}}/assets/images/LIIR_journal_club.png){:class="img-responsive" style="float: right; width:20%; margin:25px"}
Welcome to the website for the **Journal Club** at the LIIR Group. Here we will post all information about the setup
and the upcoming events. 

There are two tracks within the Journal club: the **Seminar** Sessions, and the **Reading** Group. 
In the former there are presentations from the members of the group to practice for conferences, share our work 
and give tutorials. We also occasianally host guest speakers. 

With the Reading Group we meet bi-weekly where we read and discuss some of the most important, difficult, or funny 
Papers from our fields. 

Every body is welcome to join in and participate! We also have a mailing list to inform about upcoming events. 
When we host in person, we aim to have **sandwhiches** or **cookies**! :D  
## Upcoming Events:
Here are the closest upcoming events. For a full overview, have a look at the 
[Seminar Session page]({{ "/journal-club/seminars/" | relative_url }}) or at the 
[Reading Group page]({{ "/journal-club/reading/" | relative_url }}). Here you can also find all the past events. 

#### Reading: 

| When&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Who&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | What |    
| --- | --- | --- |   
{%- assign sorted = site.data.reading_sessions | sort: 'date' -%}
{%- capture _ %}{% increment listed %}{% endcapture -%}
{%- capture nowunix %}{{ 'now' | date: '%s' }}{% endcapture -%}
{%- for article in sorted -%}
{%- capture posttime %}{{ article.date | date: '%s' }}{% endcapture -%}
{%- if posttime >= nowunix  and listed < 4 -%}
{% capture _ %}{% increment listed %}{% endcapture %}
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
{%- endif %}
{%- endfor %}
| --- | --- | --- |  

#### Seminars:

<div class="grid__wrapper">
{% assign sorted = site.seminars | sort: 'date' %}
{% capture nowunix %}{{ 'now' | date: '%s' }}{% endcapture %}
{% for post in printitems limit: 4%}
    {% capture posttime %}{{ post.date | date: '%s' }}{% endcapture %}
    {% if posttime >= nowunix %}
        {% include archive-single.html type="grid" %}
    {% endif %}
{% endfor %}
</div>

[comment]: <> ({% assign sorted = site.seminars | sort: 'date' %})

[comment]: <> ({% assign revsorted = sorted | reverse %})

[comment]: <> ({% assign futurelist = 3 %})

[comment]: <> ({% assign pastlist = 1 %})

[comment]: <> ({% capture _ %}{% increment availablefuture %}{% endcapture %})

[comment]: <> ({% capture nowunix %}{{ 'now' | date: '%s' }}{% endcapture %})

[comment]: <> ({% assign printitems = "" | split: ',' %})

[comment]: <> ({% for post in sorted %})

[comment]: <> (    {% capture posttime %}{{ post.date | date: '%s' }}{% endcapture %})

[comment]: <> (    {% if posttime >= nowunix  and availablefuture <= futurelist %})

[comment]: <> (        {% capture _ %}{% increment availablefuture %}{% endcapture %})

[comment]: <> (        {% assign printitems = printitems | append: post %})

[comment]: <> (    {% endif %})

[comment]: <> ({% endfor %})

[comment]: <> ({% assign extra = futurelist | plus: 1 | minus: availablefuture %})

[comment]: <> ({% assign pastlist = pastlist | plus: extra %})

[comment]: <> ({% assign printitems = printitems | reverse %})

[comment]: <> ({% capture _ %}{% increment selected %}{% endcapture %})

[comment]: <> ({% for post in revsorted %})

[comment]: <> (    {% capture posttime %}{{ post.date | date: '%s' }}{% endcapture %})

[comment]: <> (    {% if posttime < nowunix and selected < pastlist %})

[comment]: <> (        {% capture _ %}{% increment selected %}{% endcapture %})

[comment]: <> (        {% assign printitems = printitems | append: post %})

[comment]: <> (    {% endif %})

[comment]: <> ({% endfor %})

[comment]: <> ({% assign printitems = printitems | reverse %})
