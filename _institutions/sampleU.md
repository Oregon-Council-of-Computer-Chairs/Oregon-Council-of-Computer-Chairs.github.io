---
layout: institution  # do not change

# used to filter stale info
# make sure to change at least once a year
last_update: '2024-10-21'

name: Sample University
machine_name: sampleU
link: https://sampleuniversity.edu
image: https://www.chemeketa.edu/media/content-assets/images/student-success-stories/library-293x220.jpg
# If you have an image you want to store in the repository, place it in /assets/files/images/institutions/
# and then include it with a URL like
#image: /assets/files/images/institutions/MY_SCHOOL.png
location: Salem, OR
# Do a google maps search and then grab everything before the / that trails the 3 comma separated vales
google_location: https://www.google.com/maps/@44.9510053,-123.0029867,12.5z

# why supports multiple paragraphs. Use TWO blank lines to make a new paragraph
# ONE blank line is a line break in same paragraph
# a line break with no blank line is removed from output
#Make sure to indent all lines
why:
  Sample University is a great place. We have professors. And dorms.
  All located in beautiful downtown Salem,
  OR 97305 (same line).

  This is still the first paragraph but a new line.


  Here is a new paragraph

fte: 12242

# these are all optional
recruitment_info_link: http://google.com
transfer_info_link: http://google.com
housing_info_link: http://google.com
expected_cost_link: http://google.com

departments:
    - name: Computer Science Department
      link: https://sampleuniversity.edu/cs

      # what supports multiple lines like why: above
      what: 
        This is our department for computer science. It does things.


        It has been around for 2 months.

      annual_grads: 120

      # optional
      application_info_link: http://google.com

      # need a contact with name and (link and/or email)
      contact:
        name: CS Recruitment
        link: http://google.com
        email: x@notreal.com

      degrees:
         - name: BS Applied CS
           link: https://sampleuniversity.edu/cs/cs
           what: This is the applied degree. You can choose a focus area.
           mtm_compatible: true
           degree_requirements_link: https://sampleuniversity.edu/cs
         - name: BS in CS Systems
           link: https://sampleuniversity.edu/cs/css
           what: This is the systems degree. It focuses on low-level and theoretical computation.
           mtm_compatible: false
           degree_requirements_link: https://sampleuniversity.edu/cs


    - name: Information Systems Department
      link: https://sampleuniversity.edu/is
      what: This is our department for information systems. It builds things.
      degrees:
         - name: Mystery degree
           link: https://sampleuniversity.edu/cs/cs
           what: A mystery
           # false is the default for mtm_compatible
           # mtm_compatible: false
      # This should have more info!!!

    - name: Data Science Department
      link: https://sampleuniversity.edu/ds
      what: This is our department for information systems. It researches things.
      # this should have some degrees and other info!
---