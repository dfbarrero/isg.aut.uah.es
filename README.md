# ISG research group website
Source code of the group web site, available on http://isg.aut.uah.es/. Based on https://github.com/dfbarrero/personal-website

# Usage
1. Edit the _config.yml file to customize its settings.
2. Edit the _bibliography/references.bib file and introduce your own references. BibTeX and links are automatically generated. Available fields are: 
  - webpdf: path to the PDF file (recommended assets/pdfs)
  - dataset: path to a dataset file (recommended assets/datasets)
  - url: URL to the publisher's web page
  - slides: path to the presentation slides (recommended assets/pdfs)
  - poster: path to a poster file (recommended assets/pdfs)
3. Edit the _data/projects to customize your projects. It is self-explained.
4. Customize the home page editting _layouts/home.html.
5. Add any new section you would need. Copy any file in _pages, and use it as template to edit your own content. Insert the navigation item in _data/navigation.yml

There are some images in assets/imgs you can use as headers. Use them at your convenience.

# Deployment

Assure you have the proper Ruby development environment in your computer, with the correct versions of the libraries (bundles, in Ruby's terms): ```bundle install```.

1. Compile the website.

```
bundle exec jekyll build
```

Do not worry about the warning *Warning: Empty `slug` generated for ''.*.

2. Copy the contents of *_site* to the repository ISG-UAH/ISG-UAH.

3. Push ISG-UAH/ISG-UAH to GitHub.

# Contributors

This website has been made with Jekyll and the [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes) theme.
