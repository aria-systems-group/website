# ARIA Systems Website

## Updating Content

### News
Add a new line in `./_data/news.csv`.

### Bibliography

### Personal Pages
Add a file under `./_people/` directory.

For example

```
---
name: John Jackson                              # Your name
ordering: 2                                     # Order to be appeared in the page
email: john.m.jackson@colorado.edu              # Your Email Address
program: PhD Student                            # The program you are enrolled in
status: current                                 # Choose either current or alumnus
picture: /assets/images/john_jackson_304.jpg    # Path to your image file
picture-link: https://aerosota.com              # Your website link
header-link: https://aerosota.com               # Your website link
---
Add the introduction of yourself here.
```

### Research Pages
Similarly, you can add a new project page by creating a new markdown file under `./_projects/` directory.

```
---
name:                               # Name
layout: project                     # Leave it as it is
ordering:                           # Order to be appeared in the page
status:                             # Choose either current or past
picture:                            # Path to the image file
excerpt_separator: <!--more-->
link-flag:                          # Choose either true or false
bibkey:                             # Unique key that relates the project to some bibfiles
---

Content to be appeared in `Research` page.

<!--more-->

More detail.
```

## Updating Style
- setup Jekyll on your local machine
- clone the repo, change the branch
- make changes to style files
	- make sure they work on mobile
- open a PR so we can check

## Test Locally

Start server locally
```
bundle exec jekyll serve
```

If your ruby is missing some gems (packages), run
```
bundle install
```
