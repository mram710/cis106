---
name: Misael Ramirez-Ruiz
semester: Fall 23
course: CIS 106 Linux Fundamentals
---

# Week Report 3

## Summary of presentations

### Introduction to Linux

**What is an operating system?**

An operating system provides all fundamental software features of a computer. An OS enables you to use the computer's hardware providing you the basic tools that make the computer useful. All of those features relay on the OS's kernel. Other OS features are owed to additional programs that run atop the kernel.

**What is Ubuntu?**

Ubuntu is a Linux distribution that is freely available with both community and professional support.

**Define the following terms: Open Source, Closed Source, Free software**

Open Source: The software may be distributed for a fee or free. The source code is distributed with the software.

Closed Source: The software is not distributed with the source code. The user is restricted from modifying the code.

Free software: The software is distributed with the source code. The software can be free of charge or obtained by a fee.

**What are the 4 freedoms defined by the free software foundation?**

The first freedom known as Freedom 0 is using the software for any purpose. The second freedom known as Freedom 1 is being able to examine the source code and modify it as you see fit. The third freedom known as Freedom 2 is being able to redistribute the software. The fourth freedom known as Freedom 3 is being able to redistribute the modified software.

### The basics of Virtualization

**What is virtualization?**

Virtualization is defined as creating virtual versions of something. In this case, virtualization is used to let multiple OSs run on one physical machine at the same time.

**List 3 benefits of virtualization**

3 benefits of virtualization is being able to run multiple OSs on one machine without dual booting, allow applications to be tested before installing them on a host machine, and reduces costs by decreasing the physical hardware that must be purchased for a network.

**What is a hypervisor?**

A hypervisor is any software or hardware in charge of creating, managing, and running virtual machines.

**What is virtualbox**

VirtualBox is a powerful x86 and AMD64/Intel64 virtualization product for enterprise as well as home use. It is the only professional solution that is freely available as Open Source Software.

### Exploring Desktop Environments

**What is a desktop environment? 3 examples**

A desktop environment is an implementation of the desktop metaphor made of a bundle of programs running on top of a computer operating system, which shares a common GUI, which is sometimes described as a graphical shell. 3 examples of desktop environments are GNOME, MATE, and KDE.

**List 4 common elements of desktop environments**

4 common elements of desktop environments are icons, widgets, toolbars, and menus.

**What is Ubuntu's default desktop environments**

Ubuntu's default desktop environment is GNOME 3. The official GUI for GNOME 3 is called GNOME Shell.

**What are the official flavors of Ubuntu?**

Official flavors of Ubuntu are Xubuntu, Ubuntu Mate, Ubuntu Cinnamon, and Kubuntu.

### What is a Shell?

**What is Bash?**

The GNU bash shell is a program that provides interactive access to the Linux system. It runs as a regular program and is normally started whenever a user logs into a terminal.

**How do you access the Linux CLI?**

To access the Linux CLI you can use Terminal Emulator or the Linux Console.

**What is a console terminal?**

A console terminal is a direct interface to the Linux system that is accessed by placing the Linux system into text mode.

**What is a terminal emulator?**

A terminal emulator is a program that allows you to access the Linux CLI. 

**Provide 3 examples of Linux commands**

3 examples of Linux commands are date (displays the current time and date), cal (displays a calendar of the current month), and uname (displays information about your system).

## Managing Software

**Which command is used for updating ubuntu**

'sudo apt update; sudo apt upgrade -y'

**Which command is used for installing software? Provide example**

'sudo apt install "package name"'
example: 'sudo apt install firefox', 'sudo apt install vlc'

**Which command is used for removing software? Provide example**

'sudo apt remove "package name"'
example: 'sudo apt remove firefox', 'sudo apt remove firefox vlc'

**Which command is used for searching for software? Provide example**

'apt search "insert keyboard"'
example: 'apt search "web browser"'

**Definitions:**

**Package**

Package are archives that contain binaries of software, configuration files, and information about dependencies.

**Library**

Library are reusable codes that can be used by more than one function or program.

**Repository**

Repository is a large collection of software available for download.
