---
slug: build-a-virtual-machine
id: vsvzkj6kevae
type: challenge
title: Build a Virtual Machine
teaser: Create a temporary virtual machine where you can install software.
notes:
- type: text
  contents: Pre-installing large software components will make your track start faster
    and have fewer dependencies.
tabs:
- title: Google Project
  type: service
  hostname: cloud-client
  port: 80
difficulty: basic
timelimit: 450
---
Next you'll create a new virtual machine and install some software on it. We'll then make a custom image of the machine's disk to use in your tracks.

Follow the instructions and screenshots below to create an Ubuntu 18.04 image with the openjdk java package installed on it.

Click on the **Create Instance** buttons on the VM Instances page:

![Create Button](../assets/gcp_create_instance.png)

Next, change the name of your VM instance to **my-build-instance**:

![Name Instance](../assets/gcp_name_instance.png)

Change the boot disk for your instance to Ubuntu 18.04:

![Change Boot Disk](../assets/gcp_change_boot_disk.png)

Select Ubuntu from the pop-in menu:

![Select Ubuntu](../assets/gcp_select_ubuntu.png)

Finally click on the **Create** button at the bottom of the page:

![Click Create](../assets/gcp_create_button.png)

Once your VM has finished booting up click on the **SSH** button to connect to it. A new window will pop open with your SSH terminal connection in it.

![SSH to VM](../assets/gcp_ssh_to_vm.png)

Run the following commands to install some packages:

```bash
sudo apt -y update
sudo apt -y install git openjdk-11-jre
```

Close your terminal window and stop the VM with the **Stop** menu item. You can find it under the triple dot menu for your VM:

![Stop the VM](../assets/gcp_stop_vm.png)

Your virtual machine will gracefully shut down and the green checkmark will turn into a dark stop symbol with a square in it. Verify that your instance is stopped before going further.
