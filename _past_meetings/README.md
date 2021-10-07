# Past Meeting Records

These files are used to automatically generate pages for past meetings. The YAML
top matter defines pieces of info used by the presentation template. Freeform
content can be added below the `---`.

Any file should be added to the `/assets/files/` folder and organized by year.

Sample:

    ---
    title: Spring 2021                                       #Required
    image: /assets/files/2021/spring20.jpg                   #Optional - root relative path or full URL
    minutes: /assets/files/2021/spring2021.html              #Optional - root relative path or full URL
    location: OSU - Cascades                                 #Required
    date: 2021-04-09                                         #Required - must by yyyy-mm-dd format
    ---

    Notes about key decisions made by OCCC. New courses/degrees/etc...