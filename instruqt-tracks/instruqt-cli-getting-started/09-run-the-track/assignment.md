---
slug: run-the-track
id: dxfl3xqhyuxa
type: challenge
title: "\U0001F3C3\U0001F3FB Run the Track"
teaser: Now that you've published your first track, you can run it and test it out.
notes:
- type: text
  contents: The Instruqt development feedback cycle is fast. You can push changes
    and test them almost immediately while you are building content.
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
</style>Your new track should be up and running with your markdown instructions showing up on the assignment bar on the right. It should look just like this screenshot:

<img style="border: 1px solid;" src="https://github.com/instruqt/instruqt-training-assets/blob/master/track-images/create_a_file.png?raw=true"></img>

Fail the Check
==============

Before you run the command try out the **Check** button. You should see the expected failure message because the **hello.txt** file was not created yet.

<img style="border: 1px solid;" src="https://github.com/instruqt/instruqt-training-assets/blob/master/track-images/failed_attempt.png?raw=true"></img>

Complete the Challenge Task
===========================

Now run the command in the assignment instructions (in your new track, not this one):

```bash
echo "Hello World" > hello.txt
```

Click the **Check** button in your track again. You should see the success message now and the challenge will complete.

Since there's only one challenge the track will end here and ask you for feedback.

In the next section we'll learn how to debug and troubleshoot your track.