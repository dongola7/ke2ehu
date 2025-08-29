---
title: Repeaters
layout: default
permalink: /repeaters
---

<p>I frequently monitor the following repeaters located in and around NYC.</p>

| Location | Call | Output Frequency | Shift | Tone | Notes |
| ---      | ---  | ---              | ---   | ---  | ---   |
{%  for repeater in site.data.repeaters -%}
| {{ repeater.location }} | [{{ repeater.call }}]({{ repeater.link }}) | {{ repeater.output }} | {{ repeater.shift }} | {{ repeater.tone }} | {{ repeater.notes }} |
{% endfor -%}
