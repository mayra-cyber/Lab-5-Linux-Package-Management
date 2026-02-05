# Lab 5 — Linux Package Management

## Objective

The objective of this lab was to understand how software is managed in Linux systems by practicing installing, updating, and managing applications using Linux package managers. This lab focused on learning the difference between low-level and high-level package management tools and how repositories are used to install software and resolve dependencies.

---

## Environment

- **Host OS:** Windows  
- **VM Platform:** VirtualBox  
- **Guest OS:** Kali Linux  
- **CPU:** 2 vCPU  
- **RAM:** 2048 MB  
- **Disk:** 20 GB  

---

## Concepts Covered

### Package Management

Linux applications are distributed as packages. Package managers are used to install, remove, and manage these packages.

#### dpkg (Debian Package)
`dpkg` is a low-level package manager used to install and manage `.deb` files directly. It installs packages locally but does not automatically resolve dependencies.

#### APT (Advanced Package Tool)
APT is a higher-level package manager that communicates with online repositories to install software. It automatically downloads required dependencies and simplifies package management.

#### Repository
A repository is a remote storage location containing software packages maintained by the Linux distribution or third parties. APT retrieves packages from these repositories during installation.

---

## Steps Taken

1. Logged into the Kali Linux virtual machine.
2. Downloaded a `.deb` package (Discord) to demonstrate local package installation.
3. Navigated to the Downloads directory and verified the package.
4. Installed the package using dpkg:

```bash
sudo dpkg -i discord-0.0.111.deb

5. Updated the package repository list using:

```bash
sudo apt update

6. Installed an application using APT:

```bash
sudo apt install pidgin

7. Observed how APT automatically installed required dependencies.
8. Verified installation by launching the application from the terminal.

---

## Outcome

The installation process completed successfully. Applications were installed using both `dpkg` and `apt`, demonstrating the difference between manual package installation and automated dependency management. The virtual machine remained stable and applications launched correctly after installation.

---

## Reflection

This lab helped me understand the relationship between package managers and repositories in Linux. I learned how `dpkg` works at a lower level and why APT is commonly used for everyday software management due to its ability to handle dependencies automatically. If repeating this lab, I would also test removing packages and cleaning unused dependencies to further understand system maintenance.
