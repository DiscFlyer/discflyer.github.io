---
layout: default
---

# View my public repositories
<br />
<table>
  <colgroup>
    <col width="5%" />
    <col width="30%" />
    <col width="65%" />
  </colgroup>
  <thead>
    <tr class="header">
      <th><b>GitHub</b></th>
      <th><b>Project Name</b></th>
      <th><b>Description</b></th>
    </tr>
  </thead>
  <tbody>
    {% for repo in site.github.public_repositories %}
      <tr>
        <td><a href="{{ repo.html_url }}"><img src="assets/images/github-mark.png" width="20" height="20" /></a></td>
        <td><a href="{{ repo.homepage }}">{{ repo.name }}</a></td>
        <td>{{ repo.description }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>
