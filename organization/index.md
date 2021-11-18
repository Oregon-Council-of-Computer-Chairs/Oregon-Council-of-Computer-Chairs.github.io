---
title: Members

member_schools:
-
    name: Blue Mountain CC
-
    name: Central Oregon CC
    contacts:
    -
        name: Ken Swartwout
        email: kswartwout@cocc.edu
-
    name: Chemeketa CC
    contacts:
    -
        name: Mandy Reininger
        department: CIS
        email: mreininger@chemeketa.edu
    -
        name: Andrew Scholer
        department: CS
        email: ascholer@chemeketa.edu
        
---

There is no formal process for membership in OCCC. Every community college and public university
in Oregon is entitled to representation in the group. Many colleges send seperate representatives
for their CIS and CS programs. Below are current/recent representatives:

<table class="member-table">
<tr>
    <th>Insitution</th><th>Contact(s)</th>
</tr>
{% for school in page.member_schools %}
<tr>
    <td>{{ school.name }}</td>
    <td>
        {% if school.contacts.size > 0 %}
        <ul>
        {% for contact in school.contacts %}
        <li>
        {% if contact.email %}
            <a href="{{ member.email }}">{{ contact.name }}</a> {{ contact.department }}
        {% else %}
            {{ contact.name }} {{ contact.department }}
        {% endif %}
        </li>
        {% endfor %}
        </ul>
        {% endif %}
    </td>
</tr>
{% endfor %}
</table>





== [http://www.bluecc.edu Blue Mountain CC] ==

== [http://www.cocc.edu/ Central Oregon CC] ==

* [mailto:kswartwout@cocc.edu Ken Swartwout]

== [http://www.chemeketa.edu Chemeketa CC] ==

* [mailto:mreininger@chemeketa.edu Mandy Reininger] - CIS
* [mailto:andrew.scholer@chemeketa.edu Andrew Scholer] [http://faculty.chemeketa.edu/ascholer/] - CS

== [http://www.clackamas.edu/ Clackamas CC] ==

* [mailto:dcarino@clackamas.edu Debra Carino]
* [mailto:rcarino@clackamas.edu Rick Carino]

== [https://www.clatsopcc.edu/ Clatsop CC] ==

== [http://www.cgcc.edu/ Columbia Gorge CC] ==

* [mailto:burgess@alum.rpi.edu Robert Surton] [http://robert.surton.net/] (former)

== [http://www.oregon.gov/CCWD/ Office of Community Colleges and Workforce Development] (CCWD) ==

* [mailto:luis.juarez@state.or.us Luis Juarez]

== [http://www.eou.edu/ Eastern Oregon University] ==

*[mailto:ssheehy@eou.edu Steve Sheehy] [https://www.eou.edu/]
*[mailto:tcharrison@eou.edu Tim Harrison] [https://www.eou.edu/]

== [http://www.oregon.gov/HigherEd Higher Education Coordinating Commission] (HECC) ==

* [mailto:lisa.reynolds@state.or.us Lisa Reynolds]

== [http://www.klamathcc.edu Klamath CC] ==

* [mailto:lanning@klamathcc.edu Troy Lanning]
* [mailto:brandsness@klamathcc.edu Pete Brandsness]

== [http://lanecc.edu/ Lane CC] ==

* [mailto:coltonj@lanecc.edu Joseph Colton]

== [http://www.linnbenton.edu/ Linn-Benton CC] ==

* [mailto:jessj@linnbenton.edu Joseph Jess]*

== [http://www.mhcc.edu/ Mt. Hood CC] ==

* [mailto:deroestg@mhcc.edu Gary DeRoest]
* [mailto:Wayne.Machuca@mhcc.edu Wayne Machuca]

== [http://www.occc.cc.or.us/ Oregon Coast CC] ==

* [mailto:ebrown@occc.cc.or.us Ernest Brown]

== [http://www.oit.edu/ Oregon Institute of Technology] ==

* [mailto:Phil.Howard@oit.edu Phil Howard]
* [mailto:Todd.Breedlove@oit.edu Todd Breedlove]

== [http://eecs.oregonstate.edu/ Oregon State University] ==

* [mailto:parhammj@eecs.oregonstate.edu Jennifer Parham-Mocello]
* [mailto:calvin.hughes@oregonstate.edu Calvin Hughes]
* [mailto:yong.bakos@osucascades.edu Yong Bakos]

== [https://www.oregon.gov/HigherEd/Pages/index.aspx Oregon University System] ==

== [http://www.pcc.edu/ Portland CC] ==

* [mailto:Cara.Tang@pcc.edu Cara Tang]
* [mailto:marc.goodman@pcc.edu Marc Goodman]
* [mailto:cdjones@pcc.edu Doug Jones]
* [mailto:wmorales@pcc.edu Walter Morales] [http://spot.pcc.edu/~wmorales]

== [http://www.pdx.edu/ Portland State University] ==


* [mailto:karlaf@cs.pdx.edu Karla Fant]
* [mailto:mpj@pdx.edu Mark Jones]
* [mailto:bart@cs.pdx.edu Bart Massey]
* [mailto:warren@cs.pdx.edu Warren Harrison]

== [http://www.roguecc.edu/ Rogue CC] ==

* [mailto:jtaylor@roguecc.edu Jeremy Taylor]
* [mailto:cpatterson@roguecc.edu Cyndy Patterson]

== [http://www.sou.edu/ Southern Oregon University] ==

* [mailto:harveyd@sou.edu Dan Harvey]
* [mailto:wilson@sou.edu Dan Wilson]

== [http://www.socc.edu/ Southwestern Oregon CC] ==

* [mailto:piper.lisseveld@socc.edu Piper Lisseveld]
* [mailto:lkridelbaugh@socc.edu Linda Kridelbaugh]
* [mailto:dschab@socc.edu Diana Schab]

== [https://tillamookbaycc.edu/ Tillamook Bay CC] ==

==[https://www.tvcc.cc/ Treasure Valley CC] ==

* [mailto:jfuller@tvcc.cc Jim Fuller]
* [mailto:Kolander@tvcc.cc Budd Kolander]

== [http://www.umpqua.edu/ Umpqua CC] ==

* [mailto:john.blackwood@umpqua.edu John Blackwood]
* [mailto:vincent.yip@umpqua.edu Vincent Yip]

== [http://www.uoregon.edu/ University of Oregon] ==


* [mailto:kfreeman@cs.uoregon.edu Kathleen Freeman Hennessy]
* [mailto:cwilson@cs.uoregon.edu Chris Wilson]

== [http://www.wou.edu Western Oregon University] ==

* [mailto:morganb@wou.edu Becka Morgan] 
* [mailto:shannont@wou.edu Tad Shannon] 
