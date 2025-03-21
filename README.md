# Nessus-scan

# Nessus Scan Report - Windows 10 Machine

## Overview
This project involved conducting a Nessus vulnerability scan on a Windows 10 machine to identify potential security weaknesses, misconfigurations, and compliance issues. The scan results were analyzed to assess system security and recommend necessary remediation steps.

## Objectives
- Perform a credentialed vulnerability assessment of a Windows 10 machine.
- Identify missing patches, outdated software, and security misconfigurations.
- Detect authentication issues and network exposure risks.
- Provide actionable recommendations to enhance system security.

## Scan Details
- **Scanner:** Nessus  
- **Target System:** Windows 10  
- **Scan Type:** Credentialed Vulnerability Scan  
- **Authentication Method:** SMB (Port 445)  
- **Scan Date:** *[Insert Date]*  
- **Scan Duration:** *[Insert Duration]*  

## Key Findings
### 1. Authentication Failure - SMB Protocol (Port 445)
- **Issue:** Nessus failed to authenticate using the provided credentials (`vboxuser`).
- **Error Messages:**
  - `smb2_session_setup() failed`
  - `smb_negotiate_protocol() failed`
- **Possible Causes:**
  - Incorrect credentials
  - SMB version incompatibility
  - Firewall restrictions or disabled SMB services
- **Recommendation:**
  - Verify login credentials
  - Check SMB version compatibility (`Get-SmbServerConfiguration`)
  - Ensure SMB is enabled and accessible through firewall settings

### 2. Missing Security Updates
- **Affected Components:** *[List affected software/services]*
- **Risk Level:** *[High/Medium/Low]*
- **Recommendation:**
  - Apply Windows Updates (`Windows Update Settings` → `Check for Updates`)
  - Use WSUS or SCCM for enterprise patching

### 3. Open Ports & Network Exposure
- **Detected Open Ports:** *[List ports]*
- **Risk Level:** *[High/Medium/Low]*
- **Recommendation:**
  - Restrict unnecessary services using firewall rules
  - Implement network segmentation

## Remediation Plan
### 1. Credential Authentication Fix
   - Validate credentials used for SMB authentication
   - Configure Windows policies to allow secure credential usage

### 2. Patch Management
   - Install missing security updates and patches
   - Automate patching using Windows Update or third-party tools

### 3. Firewall & Network Security
   - Limit SMB exposure by restricting access to trusted networks
   - Disable legacy SMBv1 if not required (`Set-SmbServerConfiguration -EnableSMB1Protocol $false`)

## Conclusion
The Nessus scan provided critical insights into security gaps in the Windows 10 machine. By addressing the identified vulnerabilities, the system can be hardened against potential cyber threats. Further scans should be performed regularly to ensure ongoing security compliance.

---

## Author
**[Your Name]**  
## Date
*[Insert Date]*  
## Tools Used
- Nessus  
- PowerShell  
- Windows Security Center  

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

