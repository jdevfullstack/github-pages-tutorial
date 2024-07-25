# GitHub Pages Tutorial

*`updated July 25, 2024`*

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fxdvrx1%2Fgithub-pages-tutorial&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=PAGE+VIEWS&edge_flat=false)](https://hits.seeyoufarm.com)

## GitHub Pages
From the definition of GitHub:

> GitHub Pages is a static site hosting service designed 
to host your personal, organization, or project pages 
directly from a GitHub repository.

GitHub Pages was added when GitHub was at its early stage.
They sensed that a well-documented project is very 
important, so they simplified the process.

Take note, GitHub Pages is not a Content Management
System (CMS) like WordPress where a user can manage data
through a database and all the backend scripts
for a dynamic website but GitHub Pages can 
even be more powerful than that.

For now, even for non-technical projects, GitHub Pages
can be used to generate static web pages. Just static?
Well, from the definition of GitHub itself, you can't run
server-side scripting. But remember, Web 1.0 
was all about static web pages and we all know
the advantages of static pages against dynamic ones. 

## Why GitHub Pages?

Originally, GitHub Pages was intended for a project's
documentation. However, GitHub allows users to use it
for other purposes within certain boundaries. For
instance, creating a site to promote your business is
allowed as long as it complies with GitHub's terms of
service. Aside from those limitations, you have the
option to use GitHub Pages when you want to display
information and share it with the rest of the world,
just like a blogging site. You can even add
advertisements and donation buttons to enable financial
support.

When creating digital content, it comes in handy to use a
plaintext file. Markdown is an excellent format because
it can easily be converted into HTML, which is the
primary format consumed by web browsers.

This also encourages writers to use GitHub as their
development site because it is more efficient,
utilizing `git` to record the file's history. While
Google Docs has a similar version tracking feature,
`git` offers more robust version control capabilities.

Additionally, if you want to distribute your content as
a hard copy, you can simply right-click the page in
Google Chrome and select `Print` to generate a PDF
version of your content. If you are creating content
for another website, you can embed the page, and your
job is done. You have the repository as the active site
for development, potentially with collaboration from
others, and the GitHub Pages generated page as the
output.

If you need a Google Docs or Microsoft Word version of
your content, you can copy the rendered Markdown file
from GitHub and paste it into Google Docs or Microsoft
Word, and the format will generally remain correct with
some minor adjustments.

As you can see, using GitHub Pages is very practical.

## GitHub Pages The Easy Way
1. Create a GitHub account if there is none.

2. Create a repository or use an existing one.
For free accounts, GitHub does not allow you
to host from a private repo.

3. Initialize the repo with a `README.md`, or create one if it doesn't
   exist. This file will serve as the default landing page on GitHub.
   Other options include `index.html`, `index.htm` or `index.md`. The
   simplest method to create a web page is by using Markdown, but you
   also have the option to write in HTML if you prefer. But if you are
   writing a content, mostly you will use Markdown more than HTML.

   Note: While you can technically have `README.md`, `index.html`,
   `index.htm` and `index.md` in your repository, it's not standard
   practice to include all four. GitHub Pages will prioritize them in
   the following order: `index.html`, `index.htm`, `index.md`, and then
   `README.md`. It's best to choose one primary file for your landing
   page to avoid confusion.

4. Go to `Settings` of the repository and look for GitHub Pages
at the left side, it's just `Pages`.
   - Click `None` to trigger the dropdown.
   - Select `main` from the dropdown, it will auto-select `/root`. Leave it as is.
   - Click "Save" to apply your changes.
     <kbd><img src="https://github.com/user-attachments/assets/f907672b-8539-458e-bfae-0e0689723780" /></kbd>

5. Configure Your Site:
   - Go back to your repository.
   - Create a file named `_config.yml`.
   - Choose a theme provided by GitHub. For example:<br>
     ![Theme Selection](https://github.com/user-attachments/assets/08f71705-e35c-4fd2-b018-7b0925bfa3d2)
     
6. Visit the site provided. The URL pattern for GitHub Pages sites
typically follows this format: `https://<username>.github.io/<repository>/`.
You now have your web page.

## More Advanced Details
### GitHub Pages Root Defaults
By default, GitHub provides accounts and even Orgs a root
of your Web Page where all pages will be based from. Even if
you don't initialize this repo, you can start enabling
Pages per repo.

For a user, `<username>.github.io` is the pattern by default
so that GitHub Pages can build the site. Meaning, you should 
create a repository named after this pattern, 
so mine is `jdevfullstack.github.io`. You can now 
customize your root web page and it will be served by GitHub !
However, you may skip initializing your root directory.

### Default Documents
As was mentioned above, a default document will 
be displayed when a visitor requests
the site's URL. This is the `index.htm` file ( or `index.html`
to make sure other platforms will read it correctly )
unless you change this manually for the server to give
a different default document.

It is the same in GitHub Pages plus the `README.md`
or `index.md`.
So, when you create a repo for GitHub Pages,
you may have one default document from the three options:

- `index.htm` or `index.html`
- `README.md`
- `index.md`

When you create a subdirectory,
they are still the choices for the 
default document. The big advantage of using pure HTML
is the freedom to design your page.

### GitHub Directories for Hosting
There are three places where GitHub Pages will be building
your site from: `main`, `gh-pages` or `/docs`. 

- Using the `main`
branch, there is no additional effort, 
just set the proper configuration in `Settings`. 

- `/docs` is a subfolder of the main `branch`, 
just click `Create new file` then type 
`docs/index.htm` or any of the other
choices for the default document.
GitHub does not allow an empty folder, 
so you must initialize it with a file.
In this example, that is `index.htm`. 

- `gh-pages` is a branch, 
to create this, go to `Branch`,
type in the box `gh-pages` then hit Enter.

So, what to use ? Here are some considerations:
- if you are creating tutorial like this page of mine
you are reading, simply use the `main` branch using the 
`README.md` file. 

- the `/docs` folder is usual for those codebase with
documentation. Other document generator also relies on
this folder.

- the `gh-pages` can be your choice when your `main`
branch is dedicated for your source codes and you want
a dedicated hosting directory

- the `main` branch can be the source when it's all
about building the site not related to coding, as in
a pure Web Page

Finally, it's up to the preference of the user or the team.

### Custom Domain
Changing the default address is another story, where
you really want to make sure that you 
have an existing domain. If you know how to host 
a site from your computer,
this will be very easy for you to do. So, 
if you don't know the process yet, you find time
studying how to host a website from a different source
because the idea is the same in GitHub Pages.
I provided the link at the bottom.

### Default Themes and Custom Themes
The themes provided by GitHub Pages can be used
for your pages, just like in our example above. 
These themes will always work in Markdown files
but when you deal with pure HTML, make sure
that you always delete the head section and just include
the body so that the theme you selected will
be the one to take care of your page/s.

Then tell Jekyll that through

```
---
layout: default
---
```

on top of the HTML file.

For more information on customizing themes, visit the [GitHub Pages Documentation][github-docs].

[github-docs]: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll

## What Static Site Really Means

GitHub Pages is known for hosting static sites, but what does "static" really mean? 
Does this imply that such sites cannot incorporate dynamic elements through JavaScript?

The term "static site" refers to the way content is served to the user. In a static 
site, all content is pre-generated into HTML files and delivered directly to the 
browser. This means there's no server-side processing or database interactions 
happening in real-time when a user visits the site. 

However, this doesn't mean static sites are devoid of interactivity or dynamism. 
Through client-side JavaScript, static sites can include dynamic behaviors such as 
content updates, animations, and interactions. JavaScript can also fetch data from 
external APIs, bringing in dynamic content or functionality, albeit without direct 
server-side processing or database access on the hosting server.

The key limitation of static sites, particularly in the context of GitHub Pages, is 
the absence of backend functionality. This means while you can fetch and display 
data from external sources, you cannot directly save data back to a server or 
database through GitHub Pages. Any form of data storage or complex server-side 
logic would require external services or APIs.

In essence, static sites served through GitHub Pages offer a blend of performance 
and security for delivering content, with the flexibility to incorporate dynamic 
elements via client-side JavaScript, making them suitable for a wide range of 
applications from personal blogs to documentation and portfolio websites.
In short, it has its own advantages compared to a full-pledged website.

GitHub Pages can even host games if the code is purely written in
JavaScript. To prove this, I deployed
demo games from Vanilla Web Projects using GitHub Pages:

<https://jdevfullstack-projects.github.io/hangman-game/>

<https://jdevfullstack-projects.github.io/breakout-game/>

## Blogging Vs Vlogging
Just an added section in here since we are 
dealing with Markdown and GitHub Pages.
Do you think it's still worth writing ?

To my surprise, blogging is not dead.
I simply had that conclusion realizing
YouTube is a very successful platform.
But written content is still not dead
and it will continue to be relevant.

I just realized that blogging is not
dead because not all the contents
can be done through video presentations.
Others should be written.

Say, other tutorials are best done
through video presentations just like
bodybuilding demonstrations but
tutorials in tech, particularly just
like the full documentation of
computer languages, are best done through
text. Imagine if you will be doing
all those through video presentations,
first, that is not practical, second
it will take a lot of space and that
will be problematic for poor connection.
And third, it is best done through
writing because the content is too
complex there are several subheadings.

So, if you will be using GitHub Pages
to create written tutorials, you have
the full advantage of GitHub Pages versus
all those blogging sites.

## Useful Links
For further details, it is best to visit GitHub Pages
and other sites:

<https://pages.github.com>

<https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages>

<https://help.github.com/en/articles/user-organization-and-project-pages>

And it is important to know how GitHub Pages
differs from WordPress:

<https://viktorsmari.github.io/2019/07/14/github-pages-vs-wordpress.html> 

For my very own example, this site 

<https://jdevfullstack.github.io>

was built by GitHub Pages,
Jekyll being the static site generator. It's that simple. 

About custom domain in GitHub Pages:

<https://help.github.com/en/articles/using-a-custom-domain-with-github-pages>

## More Of My Content
- [jdevfullstack Profile](https://github.com/jdevfullstack)
- [jdevfullstack Repos](https://github.com/jdevfullstack?tab=repositories)
- [jdevfullstack Projects](https://github.com/jdevfullstack-projects)
- [jdevfullstack Tutorials](https://github.com/jdevfullstack-tutorials)
