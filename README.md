# endpoint-lab
Windows 11 and Microsoft 365 Deployment Lab Documentation
## Lab Objectives
- Plan and prepare infrastructure  
- Configure Cloud Management Gateway  
- Enroll Windows 11 devices into Microsoft Intune  
- Use Autopilot for deployment  
- Configure Windows Update for Business  
- Monitor with Endpoint Analytics  
- Apply security baselines and policies

---

## Environment Setup
### Tools Used
- Windows 11 VM (VirtualBox)
- Microsoft Endpoint Manager
- Microsoft Intune
- Configuration Manager (SCCM)
- Entra ID (Azure AD)
- Windows ADK, MDT, Windows PE

### System Requirements
- Operating System: Windows Server 2016/2019/2022, or Windows 10/11 with Hyper-V installed (recommended to use Windows Server OS) and fully updated. Administrative rights on the host. 
- Memory: 16GB RAM (32 GB RAM for optimal performance) 
- Disk Space: At least 150 GB (300 GB for optimal performance) 
- Disk Subsystem: High throughput/speed 
- TPM 2.0: TPM is required in order to enable vTPM on the VMs 
- Ethernet: Two (2) or more Gb NICs. 
- Network Connections: Internet connection and lab switch. 

- Microsoft Azure PowerShell modules installed.

---

## Step-by-Step Procedures

### 1. Infrastructure Planning
_Describe your planning process, prerequisites, and goals._

### 2. Cloud Management Gateway
_Steps to configure CMG for hybrid management._

### 3. Device Enrollment
_Manual, bulk, and Autopilot methods covered._

### 4. Policy Configuration
_Security, compliance, app protection, device restrictions._

---

## Issues Encountered & Solutions
| Issue | Solution |
|-------|----------|
| Device not enrolling in Intune | Verified MDM authority and licensing |
| CMG not connecting | Checked certs and DNS configuration |

---

## Key Skills Practiced
- Windows Autopilot Deployment  
- Device Lifecycle Management  
- MDM/MAM/UEM with Intune  
- Entra ID join & hybrid join  
- Windows update management  
- GPO vs Intune policy configuration

---

## Screenshots
_Embed screenshots using GitHub Markdown:_  
`![Description](images/screenshot1.png)`

---

## Resources & References
- [Microsoft Learn - MD-102 Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/md-102/)
- [Intune Documentation](https://learn.microsoft.com/en-us/mem/intune/)
- [SCCM Documentation](https://learn.microsoft.com/en-us/mem/configmgr/)

---

## Conclusion
_Summarize what you learned, what you'd do differently, and how this lab helps your career goal (e.g., SysAdmin or Security Analyst)._
