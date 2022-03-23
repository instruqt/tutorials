---
slug: instruqt-track-push
type: challenge
title: "\U0001F69A Instruqt Track Push"
teaser: The `instruqt track push` command will bundle up your code and push it to your organization.
notes:
  - type: text
    contents: You can push your tracks repeatedly as you develop your challenges. If you only change notes and assignment text the changes will go live immediately without restarting the track.
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
</style>Ok, we're finally ready to make our track live. Run the following command to push your new track into your organization:

```bash
instruqt track push
```

If everything went as planned you'll see the build process complete and a track URL will be shown in the output. For example:

```
Track URL: https://play.instruqt.com/instruqt/tracks/seans-new-track
```

Open this track in a new window, and proceed to the next challenge.
