# ForzaSaveSwap
A minimal, production-ready Windows tool that allows for easy swapping of Forza Horizon 5 saves.

## What this does:
- Patches a donor save to your account XUID
- Backs up your active save
- Replaces the active save with the patched donor save

## Requirements:
- Windows 10/11
- Xbox App installed (Microsoft.GamingApp.exe)
- Internet access (for Xbox profile lookup)

## Setup
- Sign into the Xbox App with the account you want to save-swap.
- Keep the Xbox App running while you use the tool.

## Usage
1. Launch ForzaSaveSwap.exe
2. Select Donor Save (the save you want to swap in)
3. Select AutoDetect of the platform youre using (Steam, MS or OnlineFix)
4. Click Grab ID to auto-fill your XUID from the signed-in Xbox App account
5. Click Save swap.

## Manual XUID option:
(Optional) Enter XUID manually to override the grabbed ID -> https://www.cxkes.me/xbox/xuid

## Auto-select buttons
- Auto-select (Steam): picks the newest Steam account folder, newest remote folder, newest .ProfileData.
- Auto-select (OnlineFix): picks the newest OnlineFix save folder and newest .ProfileData.
- Auto-select (MS Store): picks the newest WGS container save (Microsoft Store / Xbox App builds only).

## Logs
Logs are written to:

%TEMP%\ForzaSaveSwap.log
Use Open Log in the app to view.

## Backup behavior
The active save is backed up as:

<ActiveSave>.bak

## Notes
- Active save is only replaced after successful encryption. If anything fails, the original save is restored from .bak.
- Donor saves must be from FH5 v1.614.70.0 or earlier.
- You cannot saveswap a save from a newer version to an older version.

## Copyright & Distribution
This repository and its contents are provided for use only via the official GitHub source. Redistribution or sharing of the binaries outside of this GitHub repository is not authorized and violates copyright.
