---
slug: installing-the-cli
type: challenge
title: "\U0001F41A Installing the Instruqt CLI"
teaser: Download and install the Instruqt CLI on the platform of your choice.
notes:
  - type: text
    contents: |-
      **Did you know?**

      The Instruqt command line tool is written in Golang and can run on Linux, Windows, or MacOS.
tabs:
  - title: Workstation
    type: terminal
    hostname: workstation
difficulty: basic
timelimit: 300
---
<style type="text/css" rel="stylesheet">
hr.cyan { background-color: cyan; color: cyan; height: 2px; margin-bottom: -10px; }
h2.cyan { color: cyan; }
</style>The Instruqt CLI is packaged as a zip file that you can download and unzip on your workstation. You can always find the latest release of the CLI tool on our GitHub releases page:

[https://github.com/instruqt/cli/releases](https://github.com/instruqt/cli/releases)

You can also install the Instruqt CLI on your [laptop or workstation](https://docs.instruqt.com/getting-started/set-up-instruqt#step-3-set-up-your-chosen-tool). This is not required to complete the track and can be done later.

<h2 class="cyan">Install the CLI</h2>
<hr class="cyan">

Since your lab workstation runs Ubuntu Linux we'll grab the Linux version of the command line tool. Run the following command to download the Instruqt CLI zip file for Linux. You can click on the text box to copy the command. Paste the command into your Shell prompt.

```bash
wget https://github.com/instruqt/cli/releases/download/1954-00c371c/instruqt-linux-1954-00c371c.zip -O instruqt.zip
```

TIP: The keyboard shortcut **CTRL-SHIFT-P** will paste into the Shell prompt. You can also right-click in the window and select **Paste** from the menu.

Next unzip the file, make sure it's executable, and move it into the `/usr/local/bin` directory:

```bash
unzip instruqt.zip
mv instruqt /usr/local/bin/
```

Now run the following command to show the help text:

```bash
instruqt -h
```

Great work, you've installed the Instruqt CLI!
