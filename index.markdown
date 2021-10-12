---
layout: page
---

**Welcome** to our website "Getting started with open source". Who are we? A
team of pationate people contributing to open source.

<ul style="column-count: 2">
{% for people_hash in site.data.maintainers %}
{% assign people = people_hash[1] %}
  {% for person in people %}
<li>
    <a href="https://github.com/{{ member.github }}">
      {{ person.name }}
    </a>
</li>
  {% endfor %}
{% endfor %}
</ul>

This website is designed to help you open your first pull request on GitHub 🎉

The sites use Jekyll, a ruby gem, to convert Markdown files to html.
Feel free to learn more about Jekyll, ruby gems and Markdown files!

The files used to render this website are available on Github. You are tasked
with adding your name and GitHub handler to the list of the attendees. Once you
have open you first pull request and it is accepted you will be able to see
your name here.

# Attendees

<ul style="column-count: 3">
{% for people_hash in site.data.attendees %}
{% assign people = people_hash[1] %}
  {% for person in people %}
<li>
    <a href="https://github.com/{{ member.github }}">
      {{ person.name }}
    </a>
</li>
  {% endfor %}
{% endfor %}
</ul>
