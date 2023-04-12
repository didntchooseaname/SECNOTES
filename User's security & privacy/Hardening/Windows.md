
-  Set a strong password : 15 characters at least with numbers, lowercases, uppercases, specials characters
- Enable and use 2fa with biometrics or better, an hardware security key with windows Hello.
- Disable "Auto detection for proxies" in Windows and browsers (wpad protocol, NBT-NS/LLMNR poisoning)

- HardeningKitty https://github.com/0x6d69636b/windows_hardening

## 🐢 Going Further

**Follow Microsoft & NSA hardening recommendations :**

-   [Microsoft - Windows security baselines](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-security-baselines)
-   [Microsoft - Windows Server Security | Assurance](https://docs.microsoft.com/en-us/windows-server/security/security-and-assurance)
-   [Microsoft - Windows 10 Enterprise Security](https://docs.microsoft.com/en-us/windows/security/)
-   [BSI/ERNW - Configuration Recommendations for Hardening of Windows 10 Using Built-in Functionalities](https://www.bsi.bund.de/EN/Service-Navi/Publikationen/Studien/SiSyPHuS_Win10/SiSyPHuS.html?nn=1022786) (2021) - focused on Windows 10 LTSC 2019
-   [ACSC - Hardening Microsoft Windows 10, version 21H1, Workstations](https://www.cyber.gov.au/acsc/view-all-content/publications/hardening-microsoft-windows-10-version-21h1-workstations)
-   [ACSC - Securing PowerShell in the Enterprise](https://www.cyber.gov.au/publications/securing-powershell-in-the-enterprise)
-   [Awesome Windows Domain Hardening](https://github.com/PaulSec/awesome-windows-domain-hardening)
-   [Microsoft - How to detect, enable and disable SMBv1, SMBv2, and SMBv3 in Windows and Windows Server](https://support.microsoft.com/en-gb/help/2696547/detect-enable-disable-smbv1-smbv2-smbv3-in-windows-and-windows-server)
-   [Microsoft recommended block rules](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/microsoft-recommended-block-rules) - List of applications or files that can be used by an attacker to circumvent application whitelisting policies
-   [ERNW - IPv6 Hardening Guide for Windows Servers](https://www.ernw.de/download/ERNW_Guide_to_Configure_Securely_Windows_Servers_For_IPv6_v1_0.pdf)
-   [NSA - AppLocker Guidance](https://github.com/nsacyber/AppLocker-Guidance) - Configuration guidance for implementing application whitelisting with AppLocker
-   [NSA - Pass the Hash Guidance](https://github.com/nsacyber/Pass-the-Hash-Guidance) - Configuration guidance for implementing Pass-the-Hash mitigations (Archived)
-   [NSA - BitLocker Guidance](https://github.com/nsacyber/BitLocker-Guidance) - Configuration guidance for implementing disk encryption with BitLocker
-   [NSA - Event Forwarding Guidance](https://github.com/nsacyber/Event-Forwarding-Guidance) - Configuration guidance for implementing collection of security relevant Windows Event Log events by using Windows Event Forwarding
-   [Windows Defense in Depth Strategies](https://docs.google.com/document/d/1_43UroB0zY4-R2E2r_nH4ndYpDmXAY8g0oTp8yWlwBk/edit?usp=sharing) - work in progress
-   [Endpoint Isolation with the Windows Firewall](https://medium.com/@cryps1s/endpoint-isolation-with-the-windows-firewall-462a795f4cfb) based on Jessica Payne’s [‘Demystifying the Windows Firewall’](https://www.youtube.com/watch?v=InPiE0EOArs) talk from Ignite 2016

See also [Active Directory](https://github.com/decalage2/awesome-security-hardening#active-directory) and [ADFS](https://github.com/decalage2/awesome-security-hardening#adfs) below.

Source : https://github.com/decalage2/awesome-security-hardening#windows