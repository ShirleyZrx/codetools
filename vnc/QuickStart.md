# VNC Quick Start Guide

This guide provides a quick start for setting up a VNC server on Ubuntu and accessing it using a VNC viewer on Mac.

## Prerequisites

- Ubuntu machine with sudo privileges
- Mac machine

## Setting Up VNC Server on Ubuntu

1. **Install VNC Server and Desktop Environment:**
   ```bash
   sudo apt update
   sudo apt install xfce4 xfce4-goodies tightvncserver
   sudo apt install -y gnome-panel gnome-settings-daemon metacity nautilus gnome-terminal ubuntu-desktop
   sudo apt-get install tigervnc-server
   ```
2. **Configure VNC Server:**
   Start the VNC server to set up a password and create the initial configuration files:
   ```bash
   vncserver
   ```
   You will be prompted to enter a password. Make sure to remember this password as it will be used to access the VNC server.
3. **Stop the VNC Server:**
   ```bash
   vncserver -kill :1
   ```
4. **Create VNC Configuration File:**
  Edit the VNC configuration file to use the XFCE desktop environment:
  ```bash
  nano ~/.vnc/xstartup
  ```
  Replace the contents of the file with the following:
  ```bash
  #!/bin/bash
  xrdb $HOME/.Xresources
  startxfce4 &
  ```
  Make the file executable:
  ```bash
  chmod +x ~/.vnc/xstartup
  ```
5. **Start the VNC Server:**
  ```bash
  vncserver -localhost no -geometry 1920x1080 :2180  # -localhost no is a must
  vncserver -list # to list all the servers, tips: installing tigervnc-server is a must
  ```
## Accessing VNC Server from Mac
1. **Install VNC Viewer:**
   ```bash
   brew install --cask tigervnc-viewer
   ```
2. **Connect to VNC Server:**
   * Open VNC Viewer
   * Enter: ${serverIP}:${port}
   * Click "Connect"
   * Enter the password you set up earlier
You should now be connected to the VNC server running on your Ubuntu machine.

