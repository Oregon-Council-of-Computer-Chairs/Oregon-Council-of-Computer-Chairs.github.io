---
title: Course Proposals

#Edit this list to add new course proposals
#Leave date_approved blank until the course is approved
#Upload any files need to /assets/files/YEAR/
courses:
-
    number: CS290
    title: Web application development
    outline_link: /assets/files/2014/CS290.docx
    max_credits: 4
    submitter: Calvin Hughes
    submitter_email: calvin.hughes@oregonstate.edu
    institution: OSU
    date_submitted: 2014-03-05
    date_approved: 2014-05-09
-
    number: CIS242
    title: Technology Entrepreneurship
    outline_link: 
    max_credits: 3
    submitter: Chris Williamson
    submitter_email: cwilliamson@socc.edu
    institution: Southern Oregon Community College
    date_submitted: 2015-01-22
    date_approved: 2015-05-08
-
    number: CIS165
    title: Mobile application development
    outline_link: 
    max_credits: 4
    submitter: Chris Williamson
    submitter_email: cwilliamson@socc.edu
    institution: Southern Oregon Community College
    date_submitted: 2015-01-22
    date_approved: Not approved. Will use CIS234x
-
    number: CIS121
    title: Intro to Information Systems and Programming
    outline_link: /assets/files/2020/CIS121.docx
    max_credits: 4
    submitter: Marc Goodman
    submitter_email: marc.goodman@pcc.edu
    institution: Portland Community College
    date_submitted: 2019-10-19
    date_approved: 2020-04-24
-
    number: CS175
    title: Introduction to SQL
    outline_link: /assets/files/2021/Introduction_to_SQL.docx
    max_credits: 4
    submitter: Joseph Colton
    submitter_email: coltonj@lanecc.edu
    institution: Lane Community College
    date_submitted: 2021-10-18
    date_approved: 2021-10-22
---

This page is used to maintain a history of course number proposals, including descriptions, outcomes, and approval dates.

To make a proposal:

* Update this page. If you do not have write access to the github repo, send the OCCC chair a course outline including description and outcomes. ([Check the homepage for chair](../index.md))
* Once it is posted, announce the new proposal to [the OCCC mailing list](https://secure.engr.oregonstate.edu/mailman/listinfo/occc_)

Please try to make proposals two months prior to the next OCCC meeting.

<table class="course-proposal-table">
  <colgroup>
    <col>
    <col class="left">
  </colgroup>
<tr>
    <th>Number</th><th>Title</th><th>Max. Credits</th><th>Submitted by</th><th>Date Submitted</th><th>Date Approved</th>
</tr>
{% assign courses = page.courses | sort: 'date_submitted' | reverse %}
{% for course in courses %}
<tr class="{{row_class}}">
    <td>{{ course.number }}</td>
    {% if course.outline_link  %}
    <td><a href="{{ course.outline_link }}">{{ course.title }}</a></td>
    {% else %}
    <td>{{ course.title }}</td>
    {% endif %}
    <td>{{ course.max_credits }}</td>
    <td><a href="mailto:{{course.submitter_email}}">{{ course.submitter }}</a></td>
    <td>{{ course.date_submitted }}</td>
    <td>{{ course.date_approved }}</td>
</tr>
{% endfor %}
</table>