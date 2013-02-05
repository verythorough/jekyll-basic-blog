---
layout: post
title: I have a friend who asked me for help learning how to make web pages

---

# I have a friend who asked me for help learning how to make web pages
# This is my explanation

This is about choosing your first web project and getting started with it. We're going to make a Jekyll page.

First, grab a book. They're useful and give you a reliable reference. The book I recommend[^book] is [Learning Web Design: A Beginner's Guide to HTML, CSS, JavaScript, and Web Graphics](http://www.learningwebdesign.com). If you're looking for a book that is more likely to be in libraries check out [Designing With Web Standards
3rd Edition](http://www.learningwebdesign.com). This book is great, and helped bring about a bunch of great changes in the internet over the past decade. However, the third edition came out in 2009, and the web changes fast. Some of the information is outdated.

Since you have a book you can read about what the internet is, what HTML and CSS and Javascript are, and look up more terms and such. If you have a question about something, check the book first (its answers will be better) and if you can't find it there, Google it. Building web pages is mostly about looking things up on Google.

- This is written for Apple users. I talk about programs and ruby for Mac users (on OSX Lion or later). Srys.



---

### Installing things

HTML and CSS, the most basic parts of a modern web page, are just text files. You can open them with TextEdit, the text editing program that comes with OSX. But if you're planning on actually making web pages, using a text editor designed for writing code is very useful.

I recommend [Sublime Text](http://www.sublimetext.com/). It's what I use to write code every day. It's free to download, but it will nag you about purchasing it every so often. I suggest using the free trial of it until you can't stand the nag screen anymore.

You also will need to install Command Line Tools for OSX, which you can download [here](https://developer.apple.com/downloads/index.action). They are free.

You will need a Github account. Go to [Github](https://github.com/) and create an account.

Then set up Git. The easiest way to set it up is to download and install the Github application, available [here](https://central.github.com/mac/latest) [^github-assistance]. This application will only work on MacOSX Lion or Mountain Lion. If you don't have Lion or Mountain Lion I would recommend upgrading. It will make things easier.

While it would be really cool if everything could be done via a graphical interface, to get this site running we are going to have to use the terminal. [^about-the-terminal]

After you have installed the Github application, open up a terminal window. To do this, open Spotlight, the Mac OSX search utility in the upper right hand corner of the screen (Command + Spacebar is the standard keyboard shortcut) and type 'Terminal' into the search field.

This will bring up a terminal window. You should have a cursor in a blank screen.

Type `sudo gem update --system` to update your ruby gems. You will be prompted for a password. Enter your password.

Then do `gem install jekyll`[^jekyll-assistance]

Whew! You've now got everything installed to create the rockingest website evuh!

---

### Starter Site


Now you need to download the starter site. This has all of the things in it that a website needs, and offers a chance to mess around, learn things and get a feel for web sites. It's tough to create a site without some basis, and this site will provide the base for you to work from.

When you have the starter site up and running you can copy the files to a new directory and create your own site.

If you create new posts, add them to the `_posts` directory. Follow the naming conventions of the two posts in the `_posts` directory. Add the this to the top of any posts you create:

    ---
    layout: post
    title: [Put your title here]

    ---

You can look at the two sample posts to check out the way it's done.


---

### Running the site "Locally"

It's a good practice to set up any webpage you are working on on your own computer (aka locally), so you can work on pieces of it without worrying about whether you are breaking them momentarily. With Jekyll, the site generator the starter site is made with, this is incredibly easy. It might seem daunting, but compared with other options... this is a cakewalk.

Open up the terminal again, using Spotlight or whatever you find easiest.

Type `cd`

Then drag in the folder where the sample site is.

Press `enter`.

Type `jekyll --server` and hit enter again.

It's up and running!

Press `control + c` to stop it.

---

### Deploying the site (Publishing the site to the interwebs)


We're using github pages! It's free! You already have a github account! It's not confusing!

If you want to be able to view the page online make sure you push everything to a branch titled `gh-pages`. Then you will be able to access the site at.
    
    http://[your github username].[the name of the github repository].github.com

If you want to use your own domain name (so people don't visit the site at the above address, but instead go to `http://snakes-and-maps.com` or whereves) there is an explanation [here](https://help.github.com/articles/setting-up-a-custom-domain-with-pages).

__Good luck.__






[^book]: I choose this book because it was listed on [css-trick's bookshelf](http://css-tricks.com/bookshelf/). Chris Coyier, the man behind [css-tricks](css-tricks.com), is awesome and I highly recommend his site as a resource. I also purchased this book and it's a very comprehensive book with good information.

[^github-assistance]: If you have trouble installing the github app, check [here](https://help.github.com/articles/set-up-git) for their documentation.

[^jekyll-assistance]: If you have some trouble with these things, feel free to read more about how it works [here](https://github.com/mojombo/jekyll/wiki/install)

[^about-the-terminal]: I will explain how to do everything you need to do as clearly as possible, so you probably don't need to know more about the terminal. But if you run into issues, or are curious about the terminal&mdash;what it means, what it does, and how to use it&mdash;I'd recommend this [article](http://mac.tutsplus.com/tutorials/terminal/navigating-the-terminal-a-gentle-introduction/).
