---
layout: post
title: Jobs
permalink: /jobs/
---

<table>
  <thead>
    <tr>
	  <th>Title</th>
	  <th>Company</th>
	  <th>Remote</th>
	  <th>Salary</th>
	  <th>Posted</th>
	</tr>
  </thead>
  <tbody>
  {% for job in site.jobs %}
  <tr>
	  <td><a href="{{job.url}}">{{ job.job_title }}</a></td>
      <td>{{ job.company }}</td>
	  <td>{{ job.remote }}</td>
	  <td>{{ job.salary_from }} - {{job.salary_to}}</td>
	  <td>{{ job.date | date: '%d/%m/%Y' }}</td>
	</tr>
    {% endfor %}
	</tbody>
</table>
