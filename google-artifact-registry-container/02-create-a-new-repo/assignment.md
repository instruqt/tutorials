---
slug: create-a-new-repo
id: 7w4y8w18ymv8
type: challenge
title: Create a new Google Artifact Registry repo
teaser: Google Artifact Registry has replaced the legacy Google Container Registry.
  Artifact registry supports storage of many types of software artifacts including
  Docker images.
notes:
- type: text
  contents: Google container images smaller than 0.5 GB can be stored for zero cost.
    Over 0.5 GB is billed at $0.10 per GB per month.
tabs:
- title: Google Project
  type: service
  hostname: cloud-client
  port: 80
difficulty: basic
timelimit: 450
---
Create a New Repo
=================

Next you'll create a new Artifact Registry repo for storing Instruqt container images.

Click on the **Create Repository** button at the top of the page:

![Create Repository](../assets/new_repository.png)

Call your repository **instruqt-images** and select **europe-west1** for the region. You may enter an optional description, everything else can be left as defaults:

![Repo Settings](../assets/repo_settings.png)

Click on the blue **Create** button at the bottom of the page.

![Create Button](../assets/create_button.png)

You can now use this repo to store Docker images. Click **Next** to move on to the next challenge.