---
layout: page
title: Process
permalink: /process/
---

Think of this page as a sort of dashboard for all the things that go into my writing
process. Right now, it's details about the things I'm making and consuming. Over time,
it will also include summaries of feedback, polls, and other interactions with you, the
reader.

# Short Stories: 20/25

# Today's Stats
**Words written:** 1,190

**7 day average:** 1,617

**28 day average:** 1,761

**Hours spent writing:** 1.7

**7 day average:** 2

**28 day average:** 3.1

**Hours spent editing:** 0.7

**7 day average:** 1.2

**28 day average:** 1.0

# What I'm reading
{% for book in site.data.books limit:1 %}
[{{book.title}}]({{book.link}}){:target="_blank"} {% if book.recommend %}**(Recommended!)**{% else %}**(Not recommended.)**{% endif %}

{{book.blurb}}
{% endfor %}

# Everything I've read in 2019
{% for book in site.data.books %}
- [{{book.title}}]({{book.link}}){:target="_blank"}. {{book.blurb}} {% if book.recommend %}**(Recommended!)**{% else %}**(Not recommended.)**{% endif %}
{% endfor %}
