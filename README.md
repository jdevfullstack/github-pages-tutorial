# GitHub Pages Tutorial
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
Ideally, GitHub Pages was intended for a project's
documentation. However, GitHub allowed users to use
it for other purposes within the boundaries given.
For instance, creating a site to promote your business
is not allowed.
But other than those limitations, 
you have the option to use GitHub Pages
when you want to display information
and you want to share it to the rest of the world,
just like a blogging site. You can even
add an advertisement and donation button to enable 
financial support.

Remember, when you are creating a digital content,
it's better to use a plaintext file. Markdown is the
best format, as it can simply be turned into
HTML. And as we know, when it's HTML format, that's
the very consumption of web browsers, isn't it?

This also reinforces the writers to use GitHub
as their development site because it is more
efficient as it uses `git` to record the 
file's history. Even if Google Docs has a
similar version tracking, still `git`
cannot be replaced.

Now, here is the catch: when you want to distribute
your content as hard copy,
in Google Chrome, you can simply
right click the page and click `Print` 
you now have the PDF version of your content.
Also, say, you are creating content for another
website, you can simply embed the page and
your job is done. You have the repo as the 
active site for its development, maybe, others
will collaborate too, and then the GitHub Pages
generated page as the output. 
If ever you need a Google Docs
or Microsoft Word
version of this, simply copy the rendered
Markdown file of GitHub and paste it
on Google Docs or Microsoft Word, the format
will still be correct.

As you can see, it's very practical.

## How To
In the same way you keep your pages and assets in one
directory and subdirectories on the server, it is 
the same thing on GitHub Pages through a GitHub repository.

For a user, `<username>.github.io` is the pattern by default
so that GitHub Pages can build the site. Meaning, you should 
create a repository named after this pattern, 
so mine is `xdvrx1.github.io`. 
My site will be automatically created. 
However, you may skip initializing your root directory.

A default document will be displayed when a visitor requests
the site's URL. This is the `index.htm` file (or `index.html`
to make sure other platforms will read it correctly)
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

There are three places where GitHub Pages will be building
your site from: `main`, `gh-pages` or `/docs`. 

- Using the `main`
branch, there is no additional effort, 
just set the proper configuration in `Settings`. 

- `gh-pages` is a branch, 
to create this, go to `Branch`,
type in the box 'gh-pages'
then click the pop up so that
it will be created.

- `/docs` is a subfolder of the main `branch`, 
just click `Create new file` then type 
'docs/index.htm' or any of the other
choices for the default document.
GitHub does not allow empty repository, 
so you must initialize it with a file.
In this example, that is `index.htm`. 

Furthermore, as I have observed when using just a regular
account and when there is no need to change the domain name,
it's just a matter of preference and technique where you
will be building your site among the three options.

But there are few considerations:
- First, the `main` branch can be the source when it's all
about building the site.

- Second, the `gh-pages` can be your choice when your `main`
branch is dedicated for your source codes. 

- Third, the `/docs` folder is a good choice when
you want to build your site from scratch where
you don't copy the contents of the `main` branch,
as in the case of `gh-pages` branch.

Changing the default address is another story, where
you really want to make sure that you 
have an existing domain. If you know how to host 
a site from your computer,
this will be very easy for you to do. So, 
if you don't know the process yet, you find time
studying how to host a website from a different source
because the idea is the same in GitHub Pages.
I provided the link at the bottom.

The themes provided by GitHub Pages can be used
for your pages. These themes will 
always work in Markdown files
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

***
> So, the steps are:
>
> 1. Create a GitHub account if there is none.
>
> 2. Create a repository or use an existing one.
For free accounts, GitHub does not allow you
to host from a private repo.
>
> 3. Go to `Settings` and look for GitHub Pages
at the left side, it's just `Pages`.
>
> 4. Select where GitHub Pages should build 
the pages, either from:
>       - `main` (default)
>       - `gh-pages`
>       - `/docs`     
<kbd><img src="https://user-images.githubusercontent.com/47092464/115100185-abf2cd80-9f6d-11eb-85b4-1558a7335658.png" /></kbd>
> 5. And select a theme also if you want.
>
> 6. You visit the site provided. You now have your web page.

***

## The Trick
GitHub Pages generates a static site but 
don't you know that you can deploy games using this?
The trick is actually the code: if that is purely 
JavaScript, then it will work. To prove this, I deployed
demo games from Vanilla Web Projects using GitHub Pages:

<https://xdvrx1.github.io/hangman-game/>

<https://xdvrx1.github.io/breakout-game/>

As you can see here, because of the pure JavaScript,
it enables the site not to be static. Remember,
GitHub is referring to its being static 
for the server-side,
so you can't directly run, say, a PHP script. And
since JavaScript is browser-side scripting, it
will work as expected.

## Blogging Vs Vlogging
To my surprise, blogging is not dead.
I simply had that conclusion realizing
YouTube is a very successful platform.
But written content is still not dead
and it will continue to be relevant.

I just realized that blogging is not
dead because not all the contents
can be done through video presentations.
Others really need to be written.

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

<https://xdvrx1.github.io/C-Programming-Tutorial/>

was built by GitHub Pages,
Jekyll being the static site generator.
When you click `View on GitHub`, that is the repository
where all the assets and default documents reside. 
It's that simple. 

And, for those who don't know yet how to
host a site using a computer as a server,

<https://blog.mindorks.com/how-to-convert-your-laptop-desktop-into-a-server-and-host-internet-accessible-website-on-it-part-1-545940164ab9>

About custom domain in GitHub Pages:

<https://help.github.com/en/articles/using-a-custom-domain-with-github-pages>

<https://help.github.com/en/articles/custom-domain-redirects-for-github-pages-sites>
