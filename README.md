# PowerShell-guide
A comprehensive, categorized reference guide and automation utility for Windows PowerShell command aliases.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PowerShell Supported](https://img.shields.io/badge/PowerShell-5.1%20%7C%207%2B-blue)](https://microsoft.com/powershell)

A highly organized, categorized quick-reference guide for common cmdlet shortcuts and built-in aliases in Windows PowerShell. This repository aims to bridge the gap between Unix/Linux style commands and native Windows PowerShell cmdlets.

---

## 🚀 Quick Navigation
* [File System & Navigation](#-file-system--navigation)
* [File Content & Data Manipulation](#-file-content--data-manipulation)
* [System Processes & Diagnostics](#-system-processes--diagnostics)
* [Web & Networking](#-web--networking)
* [Pipeline & Core Object Mechanics](#-pipeline--core-object-mechanics)

---

## 📂 File System & Navigation

| Alias | Target Cmdlet | Functional Description |
| :--- | :--- | :--- |
| `cd` / `chdir` | `Set-Location` | Sets the current working location to a specified location. |
| `pwd` | `Get-Location` | Gets information about the current working location. |
| `dir` / `ls` / `gci` | `Get-ChildItem` | Gets the files and folders in a file system drive. |
| `md` | `mkdir` | Creates a new item (directory). |
| `copy` / `cp` / `cpi` | `Copy-Item` | Copies an item from one location to another. |
| `del` / `rm` / `erase` | `Remove-Item` | Deletes files and folders from the system. |

*(Note: Repeat this structural pattern for the remaining categories like Processes, Web Requests, and Pipeline objects.)*

---

## 🛠️ Dynamic Script Usage
This repository includes a utility script under `/scripts` to export your own local session aliases.

```powershell
# Run this to clone and test local environment aliases
./scripts/Export-CustomAlias.ps1 -ExportPath "./my-aliases.csv"
