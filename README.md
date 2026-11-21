# DoppelSpace for Power BI: downloads

A workspace for Power BI Report Server that looks and works like the Power BI service: sign-in, workspaces, apps,
per-user views and a presenter mode, on your own Windows machine. This repository holds the release downloads.

## Install in one line

On 64-bit Windows 10, Windows 11 or Windows Server, as an administrator, paste into PowerShell or the Run box:

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -Command "irm https://github.com/MYRIAD-Business-Technology/doppelspace-releases/releases/latest/download/install.ps1 | iex"
```

It downloads the latest release, checks the SHA-256 published next to it, unzips it and opens setup in an
administrator window. Setup installs SQL Server Express and Power BI Report Server from Microsoft when the machine
does not have them, creates the DoppelSpace service, asks for the first Admin account, loads two sample workspaces
and opens the browser.

## Or download the zip

Take `DoppelSpace-<version>-win64.zip` from the [latest release](https://github.com/MYRIAD-Business-Technology/doppelspace-releases/releases/latest),
unzip it, open PowerShell **as administrator** in the unzipped folder and run:

```powershell
Set-ExecutionPolicy -Scope Process Bypass -Force; .\setup.ps1
```

Each release carries a `.sha256` file for the zip. Guides are inside the zip under `docs\`.
Also available from [myriaditservices.com/doppelspace](https://myriaditservices.com/doppelspace/).

Power BI and Power BI Report Server are products of Microsoft Corporation. DoppelSpace is not affiliated with or
endorsed by Microsoft. Power BI Report Server Developer edition is licensed for development, test and demonstration only.
Built by [MYRIAD Business & Technology](https://myriaditservices.com).
