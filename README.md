Jekyll Book Boilerplate
===

A boilerplate for self-publishing books, based on the Jekyll blog platform.

Features:
- Table of contents
- Buttons for previous and next chapter
- Also, scripts for spellchecking the book and for converting it in various formats.

[See sample](https://boris-marinov.github.io/jekyll-book-boilerplate/)
===

How to use
===

If you already know how to use Jekyll, copy the boilerplate, put the chapters in the `_chapters` folder, and edit the `_config.yml`, check below for detailed steps.

Creating your book's website (in Github)
---

1. Create a Github account

2. Create a new repository from the boilerplate by following the link https://github.com/boris-marinov/jekyll-book-boilerplate/generate
3. Fill out the "Repository Name" field and click "Create" - you repository should be up on "https://github.com/<your_username>/<your_book_title>".
4. Enable Github pages
    1 Go to the profile of your repository "https://github.com/<your_username>/<your_book_title>", and click "Settings".
    2 Scroll down to the "Github pages" and under the "Source" dropdown, select "main" - you book should be up on "https://<your_username>.github.io/<your_book_title>".

Editing the chapters
===

1. Go to the `/_config.yml` file and edit the `name` and `description` fields for your book. If you are using the Github guide from above you also need to set the `baseurl` property to `<your_book_title>`.
2. In the `/_chapters` folder, place the chapters of yout book where the file names would have to follow the chapters order, like *01*, *02*, *03* etc.

Read about [Jekyll](https://jekyllrb.com/) for more info.

Converting the book to epub
===

1. Install [Pandoc](https://pandoc.org/).
2. Edit the `/title.txt` file 
3. Start the `convert` script. Under MacOS, it would work if you install GNU sed, instead of the `sed` that comes with the OS. 

There are links for downloading the epub and the txt files at the website footer 

Spellchecking
===

1. Install `npm` and the [spellchecker-cli](https://www.npmjs.com/package/spellchecker-cli) npm package.
2. Start the `spellcheck` script. 

You can fill any words that you want to exclude from the spellcheck in the `/dictionary.txt` file.
