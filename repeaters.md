---
title: Repeaters
description: Local repeaters in and around NYC
layout: default
permalink: /repeaters
---

I frequently monitor the following repeaters located in and around NYC.

| Location | Call | Output Frequency | Shift | Tone | Notes |
| ---      | ---  | ---              | ---   | ---  | ---   |
{%  for repeater in site.data.repeaters -%}
| {{ repeater.location }} | [{{ repeater.call }}]({{ repeater.link }}) | {{ repeater.output }} | {{ repeater.shift }} | {{ repeater.tone }} | {{ repeater.notes }} |
{% endfor %}

For more NYC repeaters in a [CHIRP](https://chirpmyradio.com) friendly format, see [dongola7/n2ycr_chirp](https://github.com/dongola7/n2ycr_chirp).
