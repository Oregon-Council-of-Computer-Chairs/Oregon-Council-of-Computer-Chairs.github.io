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
-
    name: Clackamas CC
    contacts:
    -
        name: Rick Carino
        department: CIS
        email: rcarino@clackamas.edu
-
    name: Clatsop CC
-
    name: Columbia Gorge CC
-
    name: Eastern Oregon University
    contacts:
    -
        name: Tim Harrison
        email: tcharrison@eou.edu
-
    name: Klamath CC
    contacts:
    -
        name: Troy Lanning
        email: lanning@klamathcc.edu
-
    name: Lane CC
    contacts:
    -
        name: Jennifer Goudreau
        email: goudreauj@lanecc.edu
-
    name: Linn-Benton CC
-
    name: Mt. Hood CC
    contacts:
    -
        name: Wayne Machuca
        department: CIS
        email: Wayne.Machuca@mhcc.edu
-
    name: Oregon Coast CC
    contacts:
    -
        name: Wayne Machuca
        department: CIS
        email: Wayne.Machuca@mhcc.edu
-
    name: Oregon Institute of Technology
    contacts:
    -
        name: Phil Howard
        department: SET Program Director
        email: Phil.Howard@oit.edu
    -
        name: Todd Breedlove
        department: CSET Chair
        email: Todd.Breedlove@oit.edu
-
    name: Oregon State University
    contacts:
    -
        name: Brett Jeter
        department: Asst. Dean - Engineering
        email: Brett.Jeter@oregonstate.edu
    -
        name: Yong Bakos
        department: OSU EECS Curriculum Committee
        email: yong.bakos@oregonstate.edu
    -
        name: Jill Hubbard
        department: OSU Cascades
        email: jill.hubbard@osucascades.edu
-
    name: Portland CC
    contacts:
    -
        name: Marc Goodman
        department: CIS
        email: marc.goodman@pcc.edu
    -
        name: Nick Insalata
        department: CS
        email: nicholas.insalata@pcc.edu
-
    name: Portland State University
    contacts:
    -
        name: Karla Fant
        department: CS
        email: karlaf@cs.pdx.edu
    -
        name: Mark Jones
        department: CS - Chair
        email: mpj@pdx.edu
-
    name: Rogue CC
-
        name: Rosie Converse
        department: CS - Chair
        email: rconverse@roguecc.edu
-
    name: Southern Oregon University
    contacts:
    -
        name: Fabrizzio Soares
        email: soaresf@sou.edu
-
    name: Southwestern Oregon CC
    contacts:
    -
        name: Maggie Vanderberg
        email: vanderbem@sou.edu
-
    name: Tillamook Bay CC
-
    name: Treasure Valley CC
-
    name: Umpqua CC
    contacts:
    -
        name: John Blackwood
        email: john.blackwood@umpqua.edu
-
    name: University of Oregon
    contacts:
    -
        name: Kathleen Freeman
        email: kfh@uoregon.edu
-
    name: Western Oregon University
    contacts:
    -
        name: Breeann Flesch
        department: CS Division Chair
        email: fleschb@wou.edu 
    -
        name: Becka Morgan
        department: CS
        email: morganb@wou.edu

---

There is no formal process for membership in OCCC. Every community college and public university
in Oregon is entitled to representation in the group. Many colleges send separate representatives
for their CIS and CS programs. Below are current/recent representatives:

<table class="member-table">
<tr>
    <th>Insitution</th><th>Contact(s)</th>
</tr>
{% assign schools = page.member_schools | sort: 'name' %}
{% for school in schools  %}
<tr>
    <td>{{ school.name }}</td>
    <td>
        {% if school.contacts.size > 0 %}
        <ul>
        {% for contact in school.contacts %}
        <li>
        {% if contact.email %}
            <a href="mailto:{{contact.email}}">{{ contact.name }}&lt;{{ contact.email }}&gt;</a>
        {% else %}
            {{ contact.name }}
        {% endif %}
        {% if contact.department %}
           - {{ contact.department }}
        {%endif %}
        </li>
        {% endfor %}
        </ul>
        {% endif %}
    </td>
</tr>
{% endfor %}
</table>
