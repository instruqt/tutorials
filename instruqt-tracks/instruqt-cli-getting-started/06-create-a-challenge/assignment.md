---
slug: create-a-challenge
id: izx4q7prjohn
type: challenge
title: "\U0001F3CB\U0001F3FB‍♀️ Create a Challenge"
teaser: Use the `instruqt challenge create` command to generate a new challenge.
notes:
- type: text
  contents: Instruqt challenges can test all kinds of skills and functions. If you
    can dream it, you can build it.
tabs:
- title: Workstation
  type: terminal
  hostname: workstation
- title: Editor
  type: code
  hostname: workstation
  path: /root
difficulty: basic
timelimit: 300
---
<style type="text/css" rel="stylesheet">
hr.cyan { background-color: cyan; color: cyan; height: 2px; margin-bottom: -10px; }
h2.cyan { color: cyan; }
</style>Instruqt tracks consist of one or more challenges that the user must complete to move forward.

Before you proceed make sure you are in your track directory, `/root/yourname-first-track`.

Create a New Challenge
======================

Create a new challenge with the following command:

```bash
instruqt challenge create --title create-a-file
```

Notice the new directory called `01-create-a-file` has appeared in your track directory. The number at the beginning of the folder determines the order in which the challenges appear in your track. If you make a mistake just delete the folder and re-create it. If you need to re-order challenges simply change the number at the beginning of the directory name.

Edit the assignment.md file
===========================

Let's take a closer look at the challenge directory. Open the `assignment.md` file in your Editor.

Notice the top section sandwiched between the triple dashes: `---`. This special section contains YAML code for configuring the current challenge. You can configure the title, description, notes, and tabs here. Tab types include Terminal, Code Editor, Service, and External Website.

Everything below the second `---` is written in Markdown. If you haven't used Markdown before, don't worry, it's really easy. Check out this cheatsheet for a quick reference and examples of what you can do with Markdown:

[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

Let's give our users some basic instructions on what to do to solve the challenge. Copy the following text into your **assignment.md** file. Note the use of triple backticks to indicate a code block that the user should run.

NOTE: This content goes at the **bottom** of the file, right below the three dashes: `---`. Copy the text below and add it to the end of the file:

<pre>
Hello user! In order to complete this challenge you'll need to create a file called **hello.txt** containing the words "Hello World". Run the following command to create the file:

```bash
echo "Hello World" > /root/hello.txt
```
</pre>

Edit the check-shell file
=========================

Now let's write a simple check script to make sure the user created the file correctly. Open the check-shell file and replace the entire file contents with the code below:

<pre>
#!/bin/bash

if ! grep "Hello World" /root/hello.txt; then
    fail-message "The hello.txt file doesn't contain the text 'Hello World'."
fi
</pre>

Save both files and proceed to the next challenge.
