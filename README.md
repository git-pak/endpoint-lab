# endpoint-lab
Windows 11 and Microsoft 365 Deployment Lab Documentation
## LAB OBJECTIVES
- Plan and prepare infrastructure  
- Configure Cloud Management Gateway  
- Enroll Windows 11 devices into Microsoft Intune  
- Use Autopilot for deployment  
- Configure Windows Update for Business  
- Monitor with Endpoint Analytics  
- Apply security baselines and policies

---

## LAB ENVIRONMENT SETUP

### LAB INTRODUCTION
This lab contains server based virtual machines and virtual hard disks. Each virtual machine contains the evaluation products installed and configured to be used in the lab. The table below lists the virtual machines, which were created and used in Hyper-V. 

| **Server Name**   | **Roles & Products**                                                                 |
|-------------------|---------------------------------------------------------------------------------------|
| **HYD-CLIENT1**   | Windows 11 24H2 Domain Joined                                                        |
| **HYD-CLIENT2**   | Windows 11 24H2 Domain Joined                                                        |
| **HYD-CLIENT3**   | Windows 11 24H2 Workgroup                                                            |
| **HYD-CLIENT4**   | Windows 11 24H2 Workgroup                                                            |
| **HYD-CLIENT 5, 6** | Bare metal (No Installations)                                                      |
| **HYD-CM1**       | Microsoft Configuration Manager 2409<br>Windows Deployment Services<br>Windows Assessment and Deployment Kit for Windows 11<br>Windows Software Update Services<br>Microsoft SQL Server 2022 |

### TOOLS USED
- Windows 11 VM (VirtualBox)
- Microsoft Endpoint Manager
- Microsoft Intune
- Configuration Manager (SCCM)
- Entra ID (Azure AD)
- Windows ADK, MDT, Windows PE

### SYSTEM REQUIREMENTS
- Operating System: Windows Server 2016/2019/2022, or Windows 10/11 with Hyper-V installed (recommended to use Windows Server OS) and fully updated. Administrative rights on the host. 
- Memory: 16GB RAM (32 GB RAM for optimal performance) 
- Disk Space: At least 150 GB (300 GB for optimal performance) 
- Disk Subsystem: High throughput/speed 
- TPM 2.0: TPM is required in order to enable vTPM on the VMs 
- Ethernet: Two (2) or more Gb NICs. 
- Network Connections: Internet connection and lab switch.
- Create an external virtual swith in hyper-v

- Microsoft Azure PowerShell modules installed.
- Licensed subscriptions for the following Microsoft Cloud Services: 
1. Microsoft Azure: https://azure.microsoft.com/en-us/free/ 
2. Enterprise Mobility + Security: http://www.microsoft.com/en-us/cloud-platform/enterprise-mobility-security-trial (configured as part of the Lab Setup below) 
3. Windows Defender for Endpoint: https://www.microsoft.com/en-us/security/business/endpoint-security/microsoft-defender-endpoint (configured as part of the Lab Setup below) 
4. Microsoft 365 E3: Configured as part of the Lab Setup below.

### SETTING UP THE LAB 

1. Created an external virtual switch in Hyper-V to provide Internet connectivity to the virtual machines. 

2. Downloaded the Win11 Lab.zip on the Hyper-V Host and extracted the contents of the ZIP file to a separate folder. 

3. Once the ZIP file was extracted, the virtual machines were imported and created into the Hyper-V Console using the provisioning Wizard in the lab. 


---


## SETTING UP AZURE AND MICROSOFT 365

### CREATING INTRA ID (formerly AZURE AD / Azure Active Directory)
1. Signed in with the email address associated with your Azure subscription. 
2. On the left navigation bar, clicked **Create a resource** > **Identity** > **Azure Active Directory**. 
3. In the Create directory pane filled in the following values: 
4. ORGANIZATION NAME: <CompanyName> 
INITIAL DOMAIN NAME: <AzureDomainName> 
COUNTRY OR REGION: Choose a region 
5. Clicked **Create**. 
(These steps are not necessary when using a free trial such as when doing this lab. Microsoft provides one free default domain) 

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
