# ARIA Systems Website

## Updating Content

### News
Add a new line in `_data/news.csv`.

### Bibliography
Add or edit entries in `_bibliography/references.bib`. The following keys are used for custom metadata:
- `url` - direct link to the paper 
- `videourl` - link to a video presentation
- `bibkey` - custom string to associate reference with project

### Personal Pages
Add a file under `_people/` directory.

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
1. First, setup Jekyll on your local machine by following the instructions here: [https://jekyllrb.com/docs/step-by-step/01-setup/](https://jekyllrb.com/docs/step-by-step/01-setup/)
2. Fork or clone the repository to your machine. 
3. To test the website locally, run `bundle exec jekyll serve` in the top directory. If there were no errors, the website will be available at http://127.0.0.1:4000/. 
4. Make changes and see how they look. Make sure changes look satisfactory on mobile devices by narrowing the browser window.
5. If you don't have direct push access, open up a pull request with your changes for review.

If your ruby is missing some gems (packages), run
```
bundle install
```
