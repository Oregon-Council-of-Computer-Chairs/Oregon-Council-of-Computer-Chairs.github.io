---
title: Past Meetings

# The past meetings page is built automatically
# See README.md in _past_meetings
---

<div id="past-meetings" class="twocols">
{% assign meetinglist = site.past_meetings %}
{% assign meetinglist = meetinglist | reverse %}
{% for meeting in meetinglist %}
<section>
<h2>{{ meeting.date | date_to_string: "ordinal", "US"  }}</h2>
<div class="meeting-details" markdown="1">
{% if meeting.minutes %}
[View Minutes]({{meeting.minutes}})
{% else %}
No minutes available
{% endif %}
</div>
<div class="meeting-contents">
</div>
<a href="{{meeting.image}}" class="meeting-pic"><img src="{{meeting.image}}"></a>
</section>
{% endfor %}
