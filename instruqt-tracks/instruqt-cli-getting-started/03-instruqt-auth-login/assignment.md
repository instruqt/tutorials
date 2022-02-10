---
slug: instruqt-auth-login
type: challenge
title: "\U0001F6C2 Log onto Instruqt"
teaser: Use the `instruqt auth login` command to authenticate yourself and safely
  store your temporary credentials.
notes:
- type: text
  contents: |-
    The Instruqt platform has a GraphQL API that you can use to manage your tracks and query data.

    https://api-docs.instruqt.com/
tabs:
- title: Workstation
  type: terminal
  hostname: workstation
- title: Login
  type: service
  hostname: workstation
  port: 15777
  new_window: true
difficulty: basic
timelimit: 300
---
<style type="text/css" rel="stylesheet">
hr.cyan { background-color: cyan; color: cyan; height: 2px; margin-bottom: -10px; }
h2.cyan { color: cyan; }
</style>For this challenge you'll need to be a member of an Instruqt organization.

Log on to Instruqt
==================

Enter the following command into your **Workstation** environment to launch the login page:
```bash
instruqt auth login
```

Now you may click on the **Login** tab. This will open a separate login window with options for authentication. If you're not sure which one to choose select "Sign in with email".

Once you have authenticated you'll see message that says:

"You are successfully logged in. You may close this browser window."

Return to the Shell
===================

Go back to your **Workstation** tab in Instruqt. If you have more than one organization you'll be asked to select which one should be the default. If you only have a single organization then it becomes the default automatically.

Nice work. You've authenticated with your Instruqt account and can begin building.

Click on the **Next** button to continue.