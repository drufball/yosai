---
layout: page
title: Process
permalink: /process/
---

Think of this page as a sort of dashboard for all the things that go into my writing
process. Right now, it's details about the things I'm making and consuming. Over time,
it will also include summaries of feedback, polls, and other interactions with you, the
reader.

# Short Stories: 1/25

# Today's Stats
**Words written:** 2,019  

**7 day average:** 1,757    

**28 day average:** Coming 3/10/19  

**Hours spent writing:** 3.2  

**7 day average:** 3.4  

**28 day average:** Coming 3/10/19  

**Hours spent editing:** 1.1  

**7 day average:** 1.3   

**28 day average:** Coming 3/10/19  

# What I'm reading
{% for book in site.data.books limit:1 %}
[{{book.title}}]({{book.link}}){:target="_blank"} {% if book.recommend %}**(Recommended!)**{% else %}**(Not recommended.)**{% endif %}

{{book.blurb}} 
{% endfor %}

# Everything I've read in 2019
{% for book in site.data.books %}
- [{{book.title}}]({{book.link}}){:target="_blank"}. {{book.blurb}} {% if book.recommend %}**(Recommended!)**{% else %}**(Not recommended.)**{% endif %}
{% endfor %}
