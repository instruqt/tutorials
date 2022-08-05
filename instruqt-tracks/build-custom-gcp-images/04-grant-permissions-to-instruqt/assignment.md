---
slug: grant-permissions-to-instruqt
id: occsnjagfhv4
type: challenge
title: Grant Permissions to Instruqt
teaser: Grant the Instruqt GCP service account read access to your GCP project.
notes:
- type: text
  contents: GCP service accounts can be used to grant read-only access to specific
    resources. Instruqt requires the Compute Image User permission to use your custom
    images in tracks.
tabs:
- title: Google Project
  type: service
  hostname: cloud-client
  port: 80
difficulty: basic
timelimit: 450
---
Important Note:
===============
The following steps no longer work in a temporary Instruqt sandbox. If you got this far in the tutorial, congratulations! The rest of the track steps explained below should be completed in your own Google Cloud Project where you plan to store your Instruqt images.

Grant Permission to Your Images
===============================

Browse to the IAM settings in your GCP console.

![GCP IAM Menu](../assets/gcp_iam_menu.png)

Create a new principal and paste the Instruqt service account email into the correct field. The Instruqt service account email is:

```
instruqt-track@instruqt-prod.iam.gserviceaccount.com
```

![Create New IAM Principal](../assets/gcp_add_iam_principal.png)

Grant the Compute Image User permission to the account and click the **Save** button.

![Grant Compute Image User Permission](../assets/gcp_add_iam_permissions.png)

That's it - now you can use your custom image in a track. Your config.yml should include the name of your project, a `/` and the name of your image. For example:

```
virtualmachines:
- name: workstation
  image: my-instruqt-project/ubuntu-openjdk-2021-12-20
  shell: /bin/bash
  machine_type: n1-standard-1
```

Remember - you'll need to repeat these steps in your company's Google organization since the Instruqt sandbox will be deleted soon.