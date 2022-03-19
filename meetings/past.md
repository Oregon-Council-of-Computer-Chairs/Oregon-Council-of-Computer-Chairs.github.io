---
title: Past Meetings

# The past meetings page is built automatically
# See README.md in _past_meetings 
---

<div id="past-meetings">
{% assign meetinglist = site.past_meetings %}
{% assign meetinglist = meetinglist | reverse %}

{% for m in meetinglist %}
    {% include_relative _meeting_template.html meeting=m %}
{% endfor %}
</div>
