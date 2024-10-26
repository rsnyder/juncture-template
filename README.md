# Juncture

Juncture is a tool for creating and displaying interactive web pages.  Juncture web pages are created using an extended version of the Markdown language.  Markdown is a lightweight markup language that is widely used to add formatting elements to plain text.  Juncture extends Markdown with the addition of a few custom tags enabling interactive viewers to be easily added to a generated web page.  Juncture uses GitHub for storing the Markdown files.

A simple Juncture-generated web page can be seen [here](https://rsnyder.github.io/juncture-template/simple-example).  This example includes a couple commonly used Juncture viewer tags.  A complete list of Juncture tags and usage examples can be found on the [Juncture documentation site](https://docs.juncture-digital.org).

## Getting Started

To begin using Juncture you will need a GitHub account and some basic familiarity with Markdown.

- *GitHub* is a free Internet hosting service commonly used for software development projects. It provides sophisticated features for version control and workflow management for distributed teams. Juncture primarily uses GitHub as a file hosting service, similar to how one might use Dropbox or Google Drive. The Markdown files that Juncture uses to render interactive web pages are stored in GitHub.  If you don't already have a GitHub account, signup for one [here](https://github.com/signup).

- *Markdown* is a simple language and a basic understanding of usage can be obtained in just a few minutes.  The [Markdown Guide - Getting Started tutorial](https://www.markdownguide.org/getting-started) is a good place to start.

### Creating your first Juncture web page

#### Configure a Juncture-enabled GitHub repository

1. **Setup GitHub repository for Juncture use**

    To display Juncture web pages some simple configuration is needed for a GitHub repository that will be used to store and display the Markdown files used by Juncture.  A new repository may be created for this purpose or an existing one may be configured.  

    - **Option 1:  Create a new Juncture-enabled GitHub repository**

        After clicking this link - [https://github.com/juncture-digital/template/generate](https://github.com/juncture-digital/template/generate)

        - Enter a Repository name (e.g,, "essays") and an optional description.
        - Press **Create Repository**

    - **Option 2:  Configure an existing GitHub repository**

        1. In the existing repository, create a Juncture template file by selecting `Create new file` from the `Add file` pull-down menu located on the repository home page.  
        2. In the file name input field enter
            ```
            _layouts/default.html
            ```
        3. In the editor section of the new file copy and paste the text displayed by this [link](https://raw.githubusercontent.com/juncture-digital/template/main/_layouts/default.html)

2. **Enable GitHub Pages on the repository**
    
    [GitHub Pages](https://pages.github.com/) is the web-page generation service provided by GitHub.  To enable GitHub Pages on a repository, select `Pages` from the `Code and automation` section in the repository `Settings` page.  In the `Pages` form select `main*` from the `Branch` pull-down menu and press `Save`.

#### Create a new Markdown file to use for the generating the web page

1. In the configured repository, create a new markdown file for the Juncture web page by selecting `Create new file` from the `Add file` pull-down menu located on the repository home page.  
2. In the file name input field enter "sunflower/index.md"
3. In the editor field add the text 
    ```
    [![](https://v3.juncture-digital.org/images/wb.svg)](https://editor.juncture-digital.org)

    # Common Sunflower

    `image wc:Sunflower_sky_backdrop.jpg .right`

    The [common sunflower](Q171497) is a species of large annual forb of the daisy family Asteraceae. The common sunflower is harvested for its edible oily seeds which are used in the production of cooking oil.
    ```
4. Press the **Commit changes...** button located at the top-right of the page.

5. To view the web page use the URL https://`<GitHub username>`.github.io/`<Github repository>`/sunflower, where `<GitHub username>` is replaced with your GitHub username and `<Github repository>` is replaced with the name of the Juncture-enabled repository containing the `sunflower/index.md` Markdown file.
