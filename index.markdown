---
layout: page
---

**Welcome** to our website "Getting started with open source". **Who are we?** Just
a team of passionate people contributing to open source projects.

**The people** behind this website are,

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

This website is designed to help you with your first pull request on GitHub 🎉

The website uses [Jekyll](https://jekyllrb.com/),
[ruby](https://www.ruby-lang.org/en/) [gem](https://rubygems.org/), to convert
[Markdown files](https://www.markdownguide.org/getting-started/) to html. Click
on any of the links if you want to learn more about Jekyll, ruby gems and
Markdown files! 😃

The files used to make this website are available on the repository
[getting-started-with-open-source](https://github.com/Nikoleta-v3/getting-started-with-open-source).
Each time you make a change to the repository the website automatically changes!

**How about you give it a try?** Add your name and GitHub handler to the list of
[attendees](https://github.com/Nikoleta-v3/getting-started-with-open-source/tree/gh-pages/_data/attendees)
and open a pull request. Once your pull request has been accepted refresh this
page to see your name!

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
