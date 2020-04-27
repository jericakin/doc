# workspace

## Welcome

This is my online resume. 

This solution is based on MkDocs. For full documentation visit [mkdocs.org](https://mkdocs.org). The Material theme for MkDocs is also applied. 

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs help` - Print this help message.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Set Up

Install python and python package handler, and then install mkdocs. This is done through the terminal, but confluence has detailed pages to step through the python parts. 

Here's the setup details. 

Set up (there will be tons of output for some of these, but that’s all good):

1. Open terminal on your Mac for CLI access. 

1. Install homebrew (copy and paste this to the command line):  

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

1. Install git.  

    brew install git

1. Your Mac probably has python 2.7 installed - so install python 3 versions:  

    brew install python3

1. Check for package upgrades:  

    pip3 install --upgrade pip

1. Install mkdocs (1.0.4).  

    pip3 install mkdocs

1. Verify a successful installation with:  

    mkdocs --version

1. Install the mkdocs material theme (4.5.0):  

    pip3 install mkdocs-material

1. Clone the doc portal repository:  

   https://git.megaport.com/documentation/workspace
   
   TechPubs is using Sourcetree as a front end to the gitlab repo. You can easily clone the repo in Sourcetree and manage/view check-ins. 
   
   http://jaredleonmorgan.net/2016/03/16/Using-Source-Tree-to-Access-Git-Lab.html

You can start a local web server with this command:

mkdocs serve

And open a browser window and go to this address:

http://127.0.0.1:8000/

**PDF Plug-in**

A few more plugins to install:

pip3 install mkdocs-markdownextradata-plugin

brew install cairo pango gdk-pixbuf libffipip3

pip3 install WeasyPrint

pip3 install mkdocs-pdf-export-plugin

brew install pandoc

**Note:** Use the brew info command to see dependencies for software packages and then install anything else needed. 

**Date Stamp Plugin**

pip3 install mkdocs-git-revision-date-localized-plugin

brew install babel

pip3 install timeago

Last update: {{ git_revision_date_localized }}

**Variable Examples:**

**{{ company.long }}**

{{ website }}

{{ vxc.short }}


