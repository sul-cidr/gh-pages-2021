# Personal & Professional Websites w/ GitHub Pages

## ![CIDR](assets/cidr.420x140.png)

## https://sul-cidr.github.io/gh-pages-2021/

---

### Before we begin...

Please sign in for this workshop at:  
https://signin.cidr.link/Websites_with_GitHub_Pages/ <!-- .element: target="signin" -->

When you've submitted the sign-in form, please keep the browser tab open on the evaluation form as a reminder to complete it when the workshop is over.

---

> This workshop will introduce you to using the free GitHub Pages service to host website and web pages online.
>
> We will take you through creating a GitHub account and a GitHub Pages site, and then show you how to create simple but useful web pages you can use to create an online presence for yourself or for a project or team.
>
> No prior experience is assumed or expected, and no special tools or software is required.

---

### Overview

<ul>
  <li class="fragment">
    Websites and Web Pages
    <ul>
      <li>HTML, CSS, and JavaScript</li>
      <li>Static Sites vs. Dynamic Sites</li>
    </ul>
  </li>

  <li class="fragment">
    Git, GitHub, and GitHub Pages
    <ul>
      <li>Concepts and Services</li>
      <li>Creating a GitHub Account</li>
    </ul>
  </li>
  <li class="fragment">
    Writing and publishing HTML pages
    <ul>
      <li>Publishing from GitHub Pages</li>
      <li>A Self-Contained Web Page</li>
      <li>A Single-Page Résumé Site</li>
    </ul>    
  </li>
  <li class="fragment">Static Site Generators, Markdown, and Jekyll</li>
</ul>

---

<!-- .slide: data-background-image="assets/html-css-javascript.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="right" -->
<!-- .slide: data-background-opacity="0.2" -->

### HTML, CSS, and Modern Web Pages

- The anatomy of a web page:
  - Content Layer (HTML)
  - Presentation Layer (CSS)
  - Behaviour Layer  
    (ECMAScript, more commonly known as JavaScript)
  - Other resources (images, media etc., potentially data)

<!-- .element class="fragment" -->

- "Static" by nature
  - Clients (web browsers) download the resources  
    and render the page on the user's computer

 <!-- .element class="fragment" -->

---

### Static vs Dynamic Websites

- **Dynamic Websites**

  - A web application creates the resources (HTML) on-demand, when a user request is made
  - Typically (though not always) involves a database server
  - Can be updated in real time, while running
  - Examples include CMSs such as WordPress, Drupal, MediaWiki

 <!-- .element class="fragment" -->

- **Static Sites**

  - Resources are created in advance of user requests and are delivered to users **exactly as stored**
  - Updates require that some or all of the pages are modified/replaced/recreated
  - No special server-side software required
  - Resources can be created by a Static Site Generator

 <!-- .element class="fragment" -->

- "Static" ≠ non-interactive!
<!-- .element class="fragment" -->

:::
Dynamic sites involve running a some software (PHP, Python, Ruby etc.) on a server somewhere

---

### Advantages of Static Sites (I)

- Security
  - Fewer (or essentially no) moving parts mean an almost non-existent attack surface

<!-- .element class="fragment" -->

- Ease of Hosting
  - The simplest possible hosting requirements mean the site can be hosted almost anywhere  
    and at little to no cost

<!-- .element class="fragment" -->

- Ease of Maintenance
  - Nothing needs regular maintenance, security patching, etc.

<!-- .element class="fragment" -->

---

### Advantages of Static Sites (II)

- Portability and Preservation/Archiving
  - Static sites are trivial to backup, to move to new locations, and to put under version control

<!-- .element class="fragment" -->

- Speed and Scalability
  - The simplicity with which static sites can be hosted also means that pages can be served  
    as fast as they can be requested

<!-- .element class="fragment" -->

- Simplicity and Control
  - With fewer moving parts and less technology between the author and final page, it's easier  
    to feel a sense of ownership and control

<!-- .element class="fragment" -->

:::

- Static sites also _require_ the author to think more in terms of simplicity which generally results in better sites (for most of the above reasons)

---

### Disadvantages of Static Sites

- Some things are more difficult and/or require third-party services and solutions
  - Site search
  - Commenting

<!-- .element class="fragment" -->

- Some things just require dynamic content
  - User-specific content
  - Working with large datasets

<!-- .element class="fragment" -->

:::
say something about widgets?

- interactive elements
- maps

---

### Static Site Generators

- The principle behind SSGs is to separate content and layout/styling ("themes")
  - This has the major advantage of avoiding repetition, and allows authors to focus on  
    the content without distractions
- Typically content is created in Markdown files

- The SSG combines the content files with a template
  - This step create the static HTML (and CSS, JavaScript etc.) files which comprise the static site
- Popular SSGs include Gatsby, Hugo, Eleventy, and Jekyll

<!-- .element class="fragment" -->

:::

---

## ![git](assets/git.png) <!-- .element class="logo-heading" -->

## ![GitHub](assets/github.png) <!-- .element class="logo-heading" -->

## ![GitHub](assets/github-pages.png) <!-- .element class="logo-heading" -->

---

<!-- .slide: data-background-image="assets/git.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

<div class="r-stack">
  <div>
    <h3>git</h3>
    <ul>
      <li>Distributed Revision Control System</li>
      <li>Created by Linus Torvalds to support Linux kernel development in 2005</li>
      <li>Completely free and open-source (GPL-2.0-only)</li>
      <li>Has a reputation for being kinda gnarly</li>
    </ul>
  </div>
  <a href="https://xkcd.com/1597/" title="XKCD - Git" target="xkcd" class="fragment"><img src="//imgs.xkcd.com/comics/git.png" title="If that doesn't fix it, git.txt contains the phone number of a friend of mine who understands git. Just wait through a few minutes of 'It's really pretty simple, just think of branches as...' and eventually you'll learn the commands that will fix everything." alt="Git" srcset="//imgs.xkcd.com/comics/git_2x.png 2x"></a>
</div>

:::
At the start of 2020:

- 2.8 million l-o-c
- ~900,000 commits
- > 27,000 contributors

---

<!-- .slide: data-background-image="assets/git.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### Some git concepts

- **Repositories**

  - For our purposes, a repository (repo) is a collection of source files that are tracked under version control.
  - Repositories can be (are) distributed -- meaning that multiple copies can exist in multiple locations

- **Commits**
  - A commit is a collection of content representing the state of the repo at a given point
  - Commits are annotated with commit messages, which typically (should) describe the changes represented by the commit

<p class="notes">Note: This is heavily simplified and omits several important concepts needed to use git effectively on your local computer.</p>

:::
This is some notes.

---

<!-- .slide: data-background-image="assets/github.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### GitHub

- Repo hosting and additional services based around git
  - Regular remote git commands
  - Issues, PRs, Wikis, GitHub Actions (CI/CD), and much more
  - GitHub Pages
- Launched in 2008, it was acquired by Microsoft in 2018
- Provides free and premium services
- At time of writing, GitHub claims [> 60 million users](https://github.com/search?q=type:user&type=Users) and [~240 million repositories](https://github.com/search)

---

<!-- .slide: data-background-image="assets/github-pages.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### GitHub Pages

- Offers free static web hosting for public GitHub repositories
  - Can serve HTML and related files directly from a repository, but can also integrate  
    SSGs to build sites from **content** in a repository
- Provides addresses of the form `<gh-user>.github.io/<repo-name>`
  - Can use custom domain names purchased and registered elsewhere
- Automatically creates free TLS (https) encryption certificates

---

<!-- .slide: data-background-image="assets/github-pages.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### Limits and Limitations of GitHub Pages

- Static sites only!

<!-- .element class="fragment" -->

- Maximum file size: 100 MB
- Maximum site size: 1 GB
- Bandwidth limit: 100 GB / month (soft limit)
- Build limit: **<mark>10 builds / hour</mark>** (soft limit)

<!-- .element class="fragment" -->

- Public sites and repositories only (on free plans)

<!-- .element class="fragment" -->

---

### Creating a GitHub Account

- Navigate to [github.com](https://github.com/) <!-- .element: target="github" --> and create an account

  - Enter the email address you want to use and choose a password
  - Complete the email verification process
  - "Skip Personalization" for now

- Complete the `README.md` repo
  - If you already had a GitHub account, create the repo `<gh-user>/<gh-user>`,  
    and create a `README.md` file
  - Edit the text a little, and make your first commit!
  - `<gh-user>/<gh-user>` is a special repo -- the contents of `README.md` will  
    appear on your GitHub profile page

---

# Let's create some websites!

---

### Create a Repository

- Create a new repository with the name `<gh-user>.github.io`

  - If you already have a repo with this name, create a new repo with whatever name you like, but be ready to make changes later on
  - Select "Add a README file" -- this will make it easier to get started

- Create a new file (<kbd>Add File</kbd> → <kbd>Create new file</kbd>) called `index.html`

  - Add some obligatory "Hello World!" text

- Navigate to <kbd>Settings</kbd> and then <kbd>Pages</kbd>, and see that your site is published

- Visit `https://<gh-user>.github.io/` and see that your site is live!

---

<!-- .slide: data-auto-animate -->

### The Simplest Possible Web Page

Copy-and-paste this simplest possible HTML document over the top of the `index.html` in your repo, and change the text. Commit the new version, and wait for GH-Pages to deploy your new page.

<pre data-id="code-animation">
  <code data-trim data-line-numbers="1|3-5|6-9|11|1-11">
    <script type="text/template">
      <html>

        <head>
          <title>Your title here...</title>
        </head>

        <body>
          Your content here...
        </body>
      
      </html>
    </script>
  </code>
</pre>

---

<!-- .slide: data-auto-animate -->

### The Simplest Possible Web Page

Copy-and-paste this simplest possible HTML document over the top of the `index.html` in your repo, and change the text. Commit the new version, and wait for GH-Pages to deploy your new page.

<pre data-id="code-animation">
  <code data-trim data-line-numbers>
    <script type="text/template">
      <html>
        
        <head>
          <title>Your title here...</title>
        </head>

        <body>
          <h1>Welcome to my page</h1> <!-- try adding a header, too! -->
          Your content here...
        </body>
      
      </html>
    </script>
  </code>
</pre>

---

### A Single-File Example

Let's create a more interesting example.

- Open the example page and take a quick look:  
  https://sul-cidr.github.io/gh-pages-2021/templates/one-file.html <!-- .element: target="one-file" -->

<!-- .element class="fragment" -->

- Use <kbd>Ctrl</kbd> + <kbd>U</kbd> or <kbd>⌘</kbd> + <kbd>U</kbd> to "View Source" and take a look at the HTML
- Copy-and-paste the entire contents over the top of your `index.html` in your repository
- Commit, and wait for the deploy

<!-- .element class="fragment" -->

---

### Using dev. tools

- Hit <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>I</kbd> or <kbd>⌘</kbd> + <kbd>Shift</kbd> + <kbd>I</kbd>
- Use the "Elements" tab (Chromium-based browsers) or the "Inspector" tab (Firefox) to take a look at the page
- Change a few things!

---

### A One-Page Résumé Site

- Check out the example  
  https://sul-cidr.github.io/gh-pages-2021/templates/one-page-resume/ <!-- .element: target="one-page-resume" -->
- Copy the page again, as before, but notice that the styles and the image are missing

<!-- .element class="fragment" -->

- Grab a zip of the whole page from:  
  https://sul-cidr.github.io/gh-pages-2021/templates/one-page-resume/one-page-resume.zip
- Extract the files to your computer somewhere, then upload them to your GitHub repo using <kbd>Add File</kbd> → <kbd>Upload files</kbd>

<!-- .element class="fragment" -->

---

### Editing with VS Code Web

- From your repo page on github.com, press the <kbd>.</kbd> key
  - The URL is the repo URL with `github.dev` in place of `github.com`

<!-- .element class="fragment" -->

- Change some text in the `index.html` file, and one or more of the colours in `style.css`, then use the <kbd>Source Control</kbd> panel to create a commit.

<!-- .element class="fragment" -->

- Desktop application (free and [mostly] open-source) can be downloaded from:  
  https://code.visualstudio.com/

<!-- .element class="fragment" -->

---

### GitHub Pages and Static Site Generators

- You can use any SSG with GitHub Pages
  - Once the pages are built (on your laptop or some other way) they are just static `.html` pages  
    (and related resources), and can be uploaded to a GitHub Pages-enabled repository just like  
    the files we've been using so far.

<!-- .element class="fragment" -->

- GitHub Pages has Jekyll built in
  - This makes it **considerably** easier to work with.

<!-- .element class="fragment" -->

---

<!-- .slide: data-background-image="assets/jekyll.svg" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### Making a site with Jekyll (I)

- Delete your `<gh-user>.github.io` repo (or rename it if you'd like to keep it around)
  - <kbd>Settings</kbd> → <kbd>Delete this repository</kbd>

<!-- .element class="fragment" -->

- Create a new repository with the same name
  - Go back to your profile page at `https://github.com/<gh-user>`, then <kbd>Repositories</kbd> → <kbd>New</kbd>

<!-- .element class="fragment" -->

- Create a new `index.md` file, with the contents

<!-- .element class="fragment" -->

```
---
title: Home
---

[Home](index.md)

# Welcome to my personal website!
```

<!-- .element class="fragment" -->

- Commit, wait for deploy, and check out your site

<!-- .element class="fragment" -->

---

<!-- .slide: data-background-image="assets/jekyll.svg" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### Making a site with Jekyll (II)

- Create a new file called `about.md`:

```
---
title: About
---

[Home](index.md) | [About](about.md)

# About me

Something about me goes here.
```

- Update `index.md` to have the extra link `[About](about.md)` too

---

<!-- .slide: data-background-image="assets/jekyll.svg" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### Front-matter and Themes with Jekyll and GitHub Pages

- Create a new file `_config.yml`:

<!-- prettier-ignore -->
```md
title: <Your Name Here>
description: Personal site for <Your Name>
remote_theme: pages-themes/hacker@v0.2.0
plugins:
  - jekyll-remote-theme
```

- Commit, wait for deploy, and check out your site

<!-- .element class="fragment" -->

- See https://github.com/pages-themes/ for the list of built-in Jekyll themes

<!-- .element class="fragment" -->

---

### Working with local files

If you do a lot of this, or if you want to get more into using git and GitHub for more than just simple static site or two, at some point you're going to need to install git on your computer and get used to keeping your local repository in sync with the remote repository (on GitHub or perhaps elsewhere).

- GitHub Desktop: https://desktop.github.com/
- https://gitforwindows.org/

---

### Further Resources (I)

- HTML / CSS

  - https://www.learn-html.org/
  - https://www.w3schools.com/
  - http://www.csszengarden.com/

- Markdown
  - https://daringfireball.net/projects/markdown/ -- The "original" markdown spec., circa 2004
  - https://guides.github.com/features/mastering-markdown/
  - https://www.markdownguide.org/

---

### Further Resources (II)

- GitHub Pages

  - https://pages.github.com/

- Jekyll

  - https://jekyllrb.com/

- GitHub Pages-supported Jekyll Themes
  - https://github.com/pages-themes/ -- officially supported themes
  - https://jekyllthemes.io/github-pages-themes

---

### Further Resources (III)

- End-to-End Tutorials for GitHub Pages and Jekyll

  - https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages
  - https://programminghistorian.org/en/lessons/collaborative-blog-with-jekyll-github

- `academicpages` is a well-known and fully-featured Jekyll theme for academics
  - https://academicpages.github.io/
  - https://jayrobwilliams.com/posts/2020/06/academic-website/

---

# Thanks! ![CIDR](assets/cidr.420x140.png)

Please fill out the evaluation form for this workshop at:
https://evaluations.cidr.link/Websites_with_GitHub_Pages/ <!-- .element: target="signin" -->

<!-- .element: style="text-align:center" -->
