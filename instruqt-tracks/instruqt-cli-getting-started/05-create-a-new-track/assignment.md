---
slug: create-a-new-track
id: iqafq8iyjhmz
type: challenge
title: "\U0001F423 Create a New Track"
teaser: Use the Instruqt CLI tool to create a brand new track.
notes:
- type: text
  contents: The Instruqt CLI creates a new track with some basic defaults. You can
    edit any of these settings once the track is created.
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
</style>In this section you'll create a new challenge for your track.

<h2 class="cyan">Create a New Track</h2>
<hr class="cyan">

Create a new track by running the following command:

```bash
instruqt track create --title "My first track"
```

A new track directory called `my-first-track` will be created and populated with track files.

<h2 class="cyan">Set Working Directory</h2>
<hr class="cyan">

Let's set your new track directory as our working directory for the rest of the lab. Run the following commands to set your working directory:

```bash
cd /root/my-first-track
set-workdir /root/my-first-track
```

This command ensures that you won't have to run the `cd` command to change into your track directory in every challenge.

<h2 class="cyan">Examine the config.yml file</h2>
<hr class="cyan">

Now hop over to the **Editor** tab and see the directory that was created for your track. Double-click the `config.yml` file inside the folder. This file is where you configure the virtual hardware that runs in your track. This may include containers, virtual machines, or cloud accounts. Currently there's only a single container called **shell**, which is running Ubuntu Linux.

<h2 class="cyan">Edit the track.yml file</h2>
<hr class="cyan">

Next, open the `track.yml` file. This file contains metadata about your track, including the title, description, and publishing settings.

Edit line 14 of the file and change the **private** line to **true**. It's a good practice to keep your track private until you're ready to share it with others. Learn more about [track access control](https://docs.instruqt.com/reference/roles-and-permissions#track-access-control) in the Instruqt docs.

You may also replace the title, teaser, and description fields if you wish. The title may have spaces in it.

Note the description field has a `|-` next to it. The pipe and hyphen indicate that a multi-line string is to follow. This allows you to write a longer description and add line breaks if you wish.

In the next section we'll create our first challenge. Click the Check button to continue.