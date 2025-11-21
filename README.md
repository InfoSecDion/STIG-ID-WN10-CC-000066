# STIG-ID-WN10-CC-000066

## Synopsis
This PowerShell script his PowerShell remediation script ensures compliance with STIG-ID WN10-CC-000066, which requires systems to audit Object Access – Removable Storage (Failure). The script configures the required advanced audit policy settings to ensure that all failed access attempts involving removable storage devices are captured in security logs.


## Notes
- **Author**: Dion Alexander
- **LinkedIn**: 
- **GitHub**: 
- **Date Created**: 2025-11-20
- **Last Modified**: 2025-11-20
- **Version**: 1.0
- **CVEs**: N/A
- **Plugin IDs**: N/A
- **STIG-ID**: WN10-CC-000066
  
## Tested On
- **Date(s) Tested**: 
- **Tested By**: 
- **Systems Tested**: 
- **PowerShell Ver.**: 

## Usage
Put any usage instructions here.

Example syntax:

```powershell
# YOUR CODE GOES HERE

# STIG-ID: WN10-CC-000066
# Requirement: Windows 10 must audit Object Access - Removable Storage (Failure)

$auditSubcategory = "Removable Storage"

# Enable Failure auditing for this advanced audit policy subcategory
auditpol /set /subcategory:"$auditSubcategory" /failure:enable

# Optional: uncomment to verify (not required by STIG, but useful in labs)
# auditpol /get /subcategory:"$auditSubcategory"
