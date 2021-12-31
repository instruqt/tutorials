---
slug: troubleshooting-and-logs
id: qudtvlxfo0nb
type: challenge
title: "\U0001F575\U0001F3FB‍♂️ Troubleshooting and Logs"
teaser: The `instruqt track logs` command can help you track down bugs and fix issues.
notes:
- type: text
  contents: When you run `instruqt track logs` from within your local track directory,
    it will show all the logs from currently running sessions of your track.
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
</style>Hit the Stop button in the Instruqt UI for your track.

Run the logs command in the Shell tab:

```bash
instruqt track logs
```

The logs for your track's build process and lifecycle scripts will begin to stream to your terminal.

Now head back over to your track URL and hit the **Start track** button.

Go back to the logs and watch the track build process. All of the output from your setup and check scripts will appear here.

This was a basic crash course to get you up and running with Instruqt. Make sure you bookmark our docs site as it contains a wealth of information and handy diagrams to help you get started:

[https://docs.instruqt.com/](https://docs.instruqt.com/)