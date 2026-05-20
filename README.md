# PowerShell-guide

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PowerShell Supported](https://img.shields.io/badge/PowerShell-5.1%20%7C%207%2B-blue)](https://microsoft.com/powershell)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen.svg)](https://github.com/your-username/powershell-alias-ref/pulls)

A comprehensive, categorized quick-reference guide and automation repository for common cmdlet shortcuts and built-in aliases in Windows PowerShell. This project bridges the gap between Unix/Linux shell commands and native Windows PowerShell cmdlets, serving as a clean cheat sheet for DevOps engineers, system administrators, and developers.

---

## 🚀 Quick Navigation
* [File System & Location Navigation](#-file-system--location-navigation)
* [File Content & Data Manipulation](#-file-content--data-manipulation)
* [System Processes, Services & Diagnostics](#-system-processes-services--diagnostics)
* [Web & Networking Requests](#-web--networking-requests)
* [Terminal Window, History & Output Formatting](#-terminal-window-history--output-formatting)
* [Core Object & Pipeline Mechanics](#-core-object--pipeline-mechanics)
* [Variables & Internal Session Aliases](#-variables--internal-session-aliases)
* [Repository Layout](#-repository-layout)
* [How to Use & Contribute](#-how-to-use--contribute)

---

## 📂 File System & Location Navigation

| Alias | Cmdlet Name | Description |
| :--- | :--- | :--- |
| `cd` / `chdir` | `Set-Location` | [cite_start]Sets the current working location to a specified location[cite: 2]. |
| `pwd` / `gl` | `Get-Location` | [cite_start]Gets information about the current working location or a location stack[cite: 6, 12]. |
| `dir` / `ls` / `gci` | `Get-ChildItem` | [cite_start]Gets the files and folders in a file system drive[cite: 2, 6, 10]. |
| `md` | `mkdir` | [cite_start]Creates a new item (directory)[cite: 10]. |
| `ni` | `New-Item` | [cite_start]Creates a new item[cite: 10]. |
| `copy` / `cp` / `cpi` | `Copy-Item` | [cite_start]Copies an item from one location to another[cite: 2]. |
| `move` / `mv` / `mi` | `Move-Item` | [cite_start]Moves an item from one location to another[cite: 10]. |
| `ren` / `rni` | `Rename-Item` | [cite_start]Renames an item in a Windows PowerShell provider namespace[cite: 12]. |
| `del` / `rm` / `rd` / `ri` / `erase` / `rmdir` | `Remove-Item` | [cite_start]Deletes files and folders[cite: 2, 4, 12]. |
| `pushd` | `Push-Location` | [cite_start]Adds the current location to the top of a location stack[cite: 12]. |
| `popd` | `Pop-Location` | [cite_start]Changes the current location to the location most recently pushed to the stack[cite: 12]. |

---

## 📄 File Content & Data Manipulation

| Alias | Cmdlet Name | Description |
| :--- | :--- | :--- |
| `cat` / `gc` | `Get-Content` | [cite_start]Gets the contents of a file[cite: 2, 6]. |
| `ac` | `Add-Content` | [cite_start]Appends content, such as words or data, to a file[cite: 2]. |
| `sc` | `Set-Content` | [cite_start]Replaces the contents of a file with contents that you specify[cite: 14]. |
| `clc` | `Clear-Content` | [cite_start]Deletes the contents of an item, but does not delete the item[cite: 2]. |
| `epcsv` | `Export-Csv` | [cite_start]Converts objects into a series of comma-separated (CSV) strings and saves them in a file[cite: 4]. |
| `ipcsv` | `Import-Csv` | [cite_start]Creates table-like custom objects from the items in a CSV file[cite: 8]. |
| `measure` | `Measure-Object` | [cite_start]Calculates the numeric properties of objects, and the characters, words, and lines in string objects[cite: 10]. |

---

## 💻 System Processes, Services & Diagnostics

| Alias | Cmdlet Name | Description |
| :--- | :--- | :--- |
| `gps` / `ps` | `Get-Process` | [cite_start]Gets the processes that are running on the local computer or a remote computer[cite: 6, 12]. |
| `saps` | `Start-Process` | [cite_start]Starts one or more processes on the local computer[cite: 14]. |
| `kill` | `Stop-Process` | [cite_start]Stops one or more running processes[cite: 10]. |
| `gsv` | `Get-Service` | [cite_start]Gets the services on a local or remote computer[cite: 8]. |
| `sasv` | `Start-Service` | [cite_start]Starts one or more stopped services[cite: 14]. |
| `gwmi` | `Get-WmiObject` | [cite_start]Gets instances of Windows Management Instrumentation (WMI) classes[cite: 8]. |

---

## 🌐 Web & Networking Requests

| Alias | Cmdlet Name | Description |
| :--- | :--- | :--- |
| `curl` / `iwr` | `Invoke-WebRequest` | [cite_start]Gets content from a webpage on the Internet[cite: 4, 8]. |
| `irm` | `Invoke-RestMethod` | [cite_start]Sends an HTTP or HTTPS request to a RESTful web service[cite: 8]. |
| `mount` / `ndr` | `New-PSDrive` | [cite_start]Creates temporary and persistent mapped network drives[cite: 10]. |
| `rdr` | `Remove-PSDrive` | [cite_start]Deletes temporary Windows PowerShell drives and disconnects mapped network drives[cite: 12]. |

---

## 🎛️ Terminal Window, History & Output Formatting

| Alias | Cmdlet Name | Description |
| :--- | :--- | :--- |
| `clear` / `cls` | `Clear-Host` | [cite_start]Clears the display in the host program[cite: 2]. |
| `echo` | `Write-Output` | [cite_start]Sends the specified objects to the next command in the pipeline[cite: 4]. |
| `ghy` / `h` / `history` | `Get-History` | [cite_start]Gets a list of the commands entered during the current session[cite: 6, 8]. |
| `ihy` / `r` | `Invoke-History` | [cite_start]Runs commands from the session history[cite: 8, 12]. |
| `clhy` | `Clear-History` | [cite_start]Deletes entries from the command history[cite: 2]. |
| `ft` | `Format-Table` | [cite_start]Formats the output as a table[cite: 6]. |
| `fl` | `Format-List` | [cite_start]Formats the output as a list of properties on new lines[cite: 4]. |
| `ogv` | `Out-GridView` | [cite_start]Sends output to an interactive table in a separate window[cite: 10]. |

---

## ⚙️ Core Object & Pipeline Mechanics

| Alias | Cmdlet Name | Description |
| :--- | :--- | :--- |
| `%` / `foreach` | `ForEach-Object` | [cite_start]Performs an operation against each item in a collection of input objects[cite: 2, 4]. |
| `?` | `Where-Object` | [cite_start]Selects objects from a collection based on their property values[cite: 2]. |
| `select` | `Select-Object` | [cite_start]Selects objects or object properties[cite: 14]. |
| `group` | `Group-Object` | [cite_start]Groups objects that contain the same value for specified properties[cite: 6]. |
| `compare` / `diff` | `Compare-Object` | [cite_start]Compares two sets of objects[cite: 2, 4]. |
| `gm` | `Get-Member` | [cite_start]Gets the properties and methods of objects[cite: 6]. |

---

## 🔑 Variables & Internal Session Aliases

| Alias | Cmdlet Name | Description |
| :--- | :--- | :--- |
| `gv` | `Get-Variable` | [cite_start]Gets the variables in the current console[cite: 8]. |
| `nv` | `New-Variable` | [cite_start]Creates a new variable[cite: 10]. |
| `set` | `Set-Variable` | [cite_start]Sets the value of a variable, creating it if it doesn't exist[cite: 14]. |
| `clv` | `Clear-Variable` | [cite_start]Deletes the value of a variable[cite: 2]. |
| `rv` | `Remove-Variable` | [cite_start]Deletes a variable and its value[cite: 14]. |
| `gal` | `Get-Alias` | [cite_start]Gets the aliases for the current session[cite: 6]. |
| `sal` | `Set-Alias` | [cite_start]Creates or changes an alias for a cmdlet or other command element[cite: 14]. |

---

## 📁 Repository Layout

```text
├── data/
│   └── aliases.json          # Structured data JSON format for integrations
├── scripts/
│   └── Export-CustomAlias.ps1 # Helper script to inspect local shell setups
├── .gitignore                # Excludes runtime session files and local OS logs
├── LICENSE                   # MIT Open-Source Certification
└── README.md                 # Project Overview & Reference Manual
