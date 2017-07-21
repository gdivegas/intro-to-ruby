---
title: Cloud 9 Environment
layout: post
date: 1000-01-02
permalink: cloud-9-environment
program: back-end
tags: back-end
---

Today, we'll be using Cloud 9 as our development environment. Cloud 9 is an online IDE (Integrated Development Environment) that will allow us to use and write Ruby code without having to download the Ruby language or a text editor. 

Check your email for an invite from Cloud 9 and follow the instructions to sign up. 

<img src="{{ site.baseurl }}/images/cloud9dashboard.png" alt="">

Let's create a new workspace. Give it a name (no spaces). Select "Don't set a team" for the workspace, and make sure to click "Blank" (not Ruby!) for the template. 

Let's look at the parts of our IDE:

<img src="{{ site.baseurl }}/images/cloud9ide.png" alt="">

<h2>The Command Line</h2>

Working in the terminal (aka command line) can be intimidating at first -- that's perfectly OK! With practice, navigation and file manipulation is significantly faster in the terminal than through a graphical interface. Professional software developers use the terminal all the time, and this class will require some use of it. 

Mac, Linux, and Windows machines all have their own command lines. Today we'll be using the built-in Cloud 9 command line.

<img src="{{ site.baseurl }}/images/terminal.png" alt="">

The line that appears in the terminal when you open it is called the prompt. It usually contains information about the user and current directory. It can be customized when not using Cloud 9.

<img src="{{ site.baseurl }}/images/commandprompt.png" alt="">

Terminal instructions often start a line with a $. This represents the last character in the prompt, you don't have to type it.

<h2>Making Files</h2>

To make a file from the command line, we use `touch filename.extension`. This will make an empty file. Use lowercase letters and no spaces for your filenames. 

To remove a file, we use `rm filename.extension`. 

Let's experiment! 

<img src="{{ site.baseurl }}/images/terminalfiles.png" alt="">

<h2>Making Folders</h2>

To make a folder from the command line, we use `mkdir foldername`. This will make an empty folder. Folders should also have lowercase letters and no spaces. Folders do not need extensions. 

Once we are inside a folder, we can make files inside that folder. 

In order to remove a folder, we need to use `rm -rf foldername` which will 

Let's experiment! 

<img src="{{ site.baseurl }}/images/terminalfolders.png" alt="">


<div class="try-it">
<h2>Try it: Terminal Practice</h2>

<p>Working in the terminal, create a directory called terminal_practice inside of the workspace. Inside the terminal_practice directory, create a file called class0.txt.</p>

<p>Practice: spend 5 minutes practicing navigating and creating/removing documents and directories with the command line. Be brave! Since we don't have anything important in this folder, it doesn't matter what you create or remove.</p>
</div>
