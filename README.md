# TAQA QuestManager — Downloads

This repository hosts **public Windows installer downloads** for **TAQA QuestManager**, the license server used by the TAQA Quest product suite.

- **Source code is not stored here.**
- Installers are **code signed**.
- **A valid QuestManager license is required** to run the service.

## What is QuestManager?
QuestManager is a **Windows-only** licensing server. After installation it runs as a **Windows Service** and allows Quest applications to authenticate against licenses hosted by your organisation.

Common deployment models:
- **Online activation** (license server checks out / validates as configured)
- **Behind-the-firewall** deployments where customers import issued licenses into their local QuestManager license server

## Download
Go to the **Releases** page for:
- the **Latest** production release, and
- prior releases (legacy versions)

Each release includes:
- the installer (MSI and/or EXE, depending on the release)
- a **SHA-256 checksum** file for integrity verification

## Verify download (SHA-256)
To verify an installer after downloading:

```powershell
Get-FileHash .\QuestManager-<version>-Setup.exe -Algorithm SHA256
```

Compare the output to the corresponding .sha256 file provided in the same GitHub Release.

## Licensing

QuestManager requires a license to run. Licenses are issued internally by TAQA and provided to customers.

If you need licensing assistance, please contact your TAQA representative or support channel.

## Legacy versions

The Releases page includes historical installers, published for convenience when customers need to match existing environments.

> Note: Legacy releases may not include newer security fixes or improvements. Use the latest release unless you have a specific compatibility requirement.
