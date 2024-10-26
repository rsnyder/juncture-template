[![](https://v3.juncture-digital.org/images/wb.svg)](https://v3.juncture-digital.org/wb)

# Juncture

Juncture is a tool for creating and displaying interactive web pages.  Juncture web pages are created using an extended version of the [Markdown](Q1193600) language.  Markdown is a lightweight markup language that is widely used to add formatting elements to plain text.  Juncture extends Markdown with the addition of a few custom tags enabling interactive viewers to be easily added to a generated web page.  Juncture uses [GitHub](Q364) for storing the Markdown files.

A simple Juncture-generated web page can be seen [here](https://rsnyder.github.io/juncture-template/simple-example).  This example includes a couple commonly used Juncture components.  A complete list of Juncture components and usage examples can be found on the [Juncture documentation site](https://docs.juncture-digital.org).

## Getting Started

To begin using Juncture you will need a GitHub account and some basic familiarity with Markdown.

**GitHub** is a free Internet hosting service commonly used for software development projects. It provides sophisticated features for version control and workflow management for distributed teams. Juncture primarily uses GitHub as a file hosting service, similar to how one might use Dropbox or Google Drive. The Markdown files that Juncture uses to render interactive web pages are stored in GitHub.

- [Signup for a free GitHub account](https://github.com/signup)

**Markdown** is a simple language and a basic understanding of usage can be obtained in just a few minutes.  Below are some resuources for learning Markdown.

- [Markdown Guide - Getting Started tutorial](https://www.markdownguide.org/getting-started)
- [markdowntutorial.com](https://www.markdowntutorial.com)
- [Markdown tutorial](https://www.youtube.com/watch?v=6A5EpqqDOdk)

### Creating your first Juncture web page

#### Configure a Juncture-enabled GitHub repository

1. **Setup GitHub repository for Juncture use**

    To display Juncture web pages some simple configuration is needed for a GitHub repository that will be used to store and display the Markdown files used by Juncture.  A new repository may be created for this purpose or an existing one may be configured.  

    - **Option 1:  Create a new Juncture-enabled GitHub repository**

        Using this link - [https://github.com/juncture-digital/template/generate](https://github.com/juncture-digital/template/generate)

        - Enter a Repository name (e.g,, "essays") and optional Description.
        - Press **Create Repository**

    - **Option 2:  Configure an existing GitHub repository**

        1. In the existing repository, create a Juncture template file by selecting `Create new file` from the `Add file` pull-down menu located on the repository home page.  
        2. In the file name input field enter "_layouts/default.html".
        3. In the editor section of the new file add the text displayed after clicking this [link](https://raw.githubusercontent.com/juncture-digital/template/main/_layouts/default.html)

2. **Enable GitHub Pages on the repository**
    
    GitHub Pages is the web-page generation service provided by GitHub.  To enable GitHub Pages, select `Pages` from the `Code and automation` section in the repository `Settings` page.  In the `Pages` form select `main*` from the `Branch` pull-down menu and press `Save`.

#### Create a new Markdown file to use for the Juncture essay

1. In the configured repository, create a new markdown file for the Juncture web page by selecting `Create new file` from the `Add file` pull-down menu located on the repository home page.  
2. In the file name input field enter "sunflower/index.md"
3. In the editor field add the text 
    ```
    [![](https://v3.juncture-digital.org/images/wb.svg)](https://editor.juncture-digital.org)
    ```
4. Press the **Commit changes...** button located at the top-right of the page.

#### Add Markdown text for your Juncture page

At this point you should have a new repository with a `index.md` file located in a folder named `sunflower`.

To add Juncture-augmented Markdown text for the generated web page you may continue to use the GitHub editor or use the Juncture editor.  The Juncture editor is recommended as it provides syntax-highlighting, a preview toggle for rapidly making and viewing changes.  The instructions in this Getting Started guide assume the Juncture editor is being used.

To access the editor, press the two-toned "Juncture Workbench" button now displayed at the top of the Markdown file when viewing from the GitHub site.  The first time the Juncture editor is used you'll be asked to authorize Juncture to access your repository.

Append the following text to your `sunflower/README.md` file, leaving a blank line after the button text added in the previous step.

```
# Common Sunflower

`image wc:Sunflower_sky_backdrop.jpg .right`

The [common sunflower](Q171497) is a species of large annual forb of the daisy family Asteraceae. The common sunflower is harvested for its edible oily seeds which are used in the production of cooking oil.
```
	
After adding the new text, press the preview button (the eye icon) located in the editor toolbar to view the rendered web page.

