---
slug: instruqt-track-validate
id: pignumomi5mz
type: challenge
title: ☑️ Instruqt Track Validate
teaser: Use the `instruqt track validate` command to verify your track code.
notes:
- type: text
  contents: The validate command can be used in CI/CD pipelines to fail fast when
    invalid configurations are detected.
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
</style>Run the following command from within your track directory:

```bash
instruqt track validate
```

If all goes well you should see a bunch of **OK** messages. This means it's ok to proceed to the next challenge.