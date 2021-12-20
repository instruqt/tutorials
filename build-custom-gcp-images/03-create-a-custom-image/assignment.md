---
slug: create-a-custom-image
id: fk0l8xk4kgtw
type: challenge
title: Create a Custom Image
teaser: Make a copy of the build machine's startup disk for use in your Instruqt tracks.
notes:
- type: text
  contents: Instruqt uses custom images or simply "Images". The GCP "Machine Image"
    is not suitable for use in Instruqt tracks.
tabs:
- title: Google Project
  type: service
  hostname: cloud-client
  port: 80
# - title: Workstation
#   type: terminal
#   hostname: workstation
difficulty: basic
timelimit: 600
---
If you've come from AWS you might be familiar with the concept of an Amazon Machine Image (AMI).

On GCP things are a bit different. GCP Machine Images are a collection of OS, disks, metadata and settings that can be used to take an exact backup of a running machine.

Instruqt uses plain Images, also known as Custom Images, to create virtual machines.

In the next step make sure you select **Images** and not **Machine Images**.

![Custom Images Menu](../assets/gcp_custom_images_menu.png)

At the top of the page select the **Create Image** button:

![Create Image Button](../assets/gcp_create_image_button.png)

Give the image a descriptive name. In this example we'll use `ubuntu-openjdk-2021-12-20`.

Under **Source Disk** select the disk from **my-build-instance**.

![Custom Image Name](../assets/gcp_custom_image_name.png)

Then set the **Location** to **Regional** and select **europe-west1**.

![Image Region](../assets/gcp_image_region.png)

Optional: You may put more details into the **Description** field if you wish.

Finally click the **Create** button at the bottom of the page. It will take a minute or two for your custom image to be built. You'll know it's done when there's a green checkmark in the **Status** column:

![Completed Image](../assets/gcp_completed_image.png)

Your new custom image is ready to use! Go to the next challenge to learn how to set up permissions for Instruqt to use the image.