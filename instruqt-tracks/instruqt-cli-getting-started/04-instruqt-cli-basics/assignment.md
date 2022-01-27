---
slug: instruqt-cli-basics
type: challenge
title: "\U0001F469\U0001F3FE‍\U0001F3EB Instruqt CLI Basics"
teaser: Learn some basic Instruqt CLI commands.
notes:
- type: text
  contents: The Instruqt CLI can be used on your laptop, or by CI/CD tools for automated
    builds and testing.
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
</style>Let's try a few basic commands. The first one you've already seen:

```bash
instruqt -h
```

When you add an `-h` flag it will show more information about the command or subcommand.

Check your command line configuration settings:

```bash
instruqt config list
```

This command will show all the configuration properties of the CLI, including your current default organization. Take a moment to confirm that you have configured the correct organization with the CLI.

You can view the version of the Instruqt CLI with this command:

```bash
instruqt version
```

Next let's check for updates:

```bash
instruqt update
```

The Instruqt CLI can automatically update itself on most systems. It automatically checks for new versions each time you start it up.

Now that you have a feel for the command line tool, let's create our first track. Hit the **Next** button below to proceed.
