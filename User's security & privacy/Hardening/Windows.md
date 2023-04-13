
### :luc_mouse_pointer_click: Mandatory zone (do first)
-  Encrypt your whole drives with bitlocker.
- Enable SecureBoot and put a password on the bios.
- Set a strong password for your login account : 15 characters at least with numbers, lowercases, uppercases, specials characters.
- Enable and use 2fa with biometrics or better, an hardware security key with windows Hello.
- Disable "Auto detection for proxies" in Windows and browsers (wpad protocol, NBT-NS/LLMNR poisoning).

### :luc_server_crash: Mandatory security : 

- [ ]  ([Secure-Core](https://learn.microsoft.com/en-us/windows-hardware/design/device-experiences/oem-highly-secure))
- [ ] Be sure that Windows is [up-to-date](https://www.microsoft.com/en-us/software-download/windows11)
- [ ] Be sure that Microsoft Defender is [up-to-date](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/manage-updates-baselines-microsoft-defender-antivirus?view=o365-worldwide#monthly-platform-and-engine-versions)
- [ ] Be sure that Latest Driver and Program are updated
- [ ] Only necessary programs/apps/games which you need
- [ ] stay away from "Anti-Spying"/"Anti-Telemetry"/.. tools and use [official documentation](https://github.com/beerisgood/Windows11_Privacy)
- [ ] [Hardware Requirements](https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-defender-system-guard/system-guard-secure-launch-and-smm-protection#requirements-met-by-system-guard-enabled-machines) for [System Guard](https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-defender-system-guard/how-hardware-based-root-of-trust-helps-protect-windows) / [Hardware-based Isolation](https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-defender-system-guard/how-hardware-based-root-of-trust-helps-protect-windows?view=o365-worldwide)
- [ ] [Hardware Requirements](https://learn.microsoft.com/en-us/windows/security/threat-protection/device-guard/requirements-and-deployment-planning-guidelines-for-virtualization-based-protection-of-code-integrity#baseline-protections) for [Memory integrity](https://support.microsoft.com/en-us/windows/core-isolation-e30ed737-17d8-42f3-a2a9-87521df09b78)
- [ ] [Hardware Requirements](https://learn.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard) for Microsoft [Defender Application Guard](https://learn.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-application-guard/md-app-guard-overview) (WDAG)
- [ ] [Hardware Requirements](https://learn.microsoft.com/en-us/windows/security/identity-protection/credential-guard/credential-guard-requirements) for Microsoft [Defender Credential Guard](https://learn.microsoft.com/en-us/windows/security/identity-protection/credential-guard/credential-guard-how-it-works)


### :luc_lock: Hardening
- [ ] Set User Account Control ([UAC](https://learn.microsoft.com/en-us/windows/security/identity-protection/user-account-control/user-account-control-overview)) to [maximum](https://github.com/beerisgood/Windows11_Hardening/blob/master/maximum%20UAC%20level)
- [ ] [Create](https://support.microsoft.com/en-us/windows/create-a-local-user-or-administrator-account-in-windows-20de74e0-ac7f-3502-a866-32915af2a34d) a different Admin account and [transform](https://www.windowscentral.com/how-change-user-account-type-windows-10/3) your current account to limited/restricted/standard user to reduce the attack surface enormously. Don't use administrator access for your tasks!
- [ ] Use [Smart App Control](https://support.microsoft.com/en-us/topic/what-is-smart-app-control-285ea03d-fa88-4d56-882e-6698afdb7003)
- [ ] [Block all incoming connections](https://malwaretips.com/threads/what-would-happen-if-a-legimate-program-os-or-game-somehow-had-a-virus-or-malware-installed-on-it-from-the-official-source.108861/page-2#post-949038) with Microsoft Defender Firewall
- [ ] Always [display file type extension](https://github.com/beerisgood/Windows11_Hardening/blob/master/always%20display%20file%20type%20extension)
- [ ] [Manage](https://learn.microsoft.com/en-us/windows/security/identity-protection/credential-guard/credential-guard-manage) Microsoft Defender [Credential Guard](https://learn.microsoft.com/en-us/windows/security/identity-protection/credential-guard/credential-guard)
- [ ] Install Microsoft Defender Application Guard ([WDAG](https://learn.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-application-guard/install-md-app-guard#install-application-guard)) and use it for untrusted sites
- [ ] Enable Memory Integrity ([HVCI](https://learn.microsoft.com/en-us/windows/security/threat-protection/device-guard/enable-virtualization-based-protection-of-code-integrity#how-to-turn-on-hvci-in-windows-10))
- [ ] Enable Network Protection ([NP](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/network-protection?view=o365-worldwide))
- [ ] Enable [SmartScreen](https://learn.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-smartscreen/microsoft-defender-smartscreen-set-individual-device) and enable [SmartScreen Logs](https://learn.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-smartscreen/microsoft-defender-smartscreen-overview#viewing-windows-event-logs-for-windows-defender-smartscreen)
- [ ] Enable Controlled Folder Access ([CFA](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/controlled-folders?view=o365-worldwide))
- [ ] Enable Attack Surface Reduction rules ([ASR](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/attack-surface-reduction-rules-reference?view=o365-worldwide))
- [ ] [Enable](https://github.com/beerisgood/Windows11_Hardening/blob/master/harden%20ASLR) Mandatory ALSR and Bottom-Up-ALSR ([Address Space Layout Randomization](https://docs.microsoft.com/en-us/windows/security/threat-protection/overview-of-threat-mitigations-in-windows-10#address-space-layout-randomization))
- [ ] Enable [System Guard Secure Launch](https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-defender-system-guard/system-guard-secure-launch-and-smm-protection#windows-security-center)
- [ ] Enable [cloud-delivered protection](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/enable-cloud-protection-microsoft-defender-antivirus?view=o365-worldwide)
- [ ] [Enable](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/detect-block-potentially-unwanted-apps-microsoft-defender-antivirus?ocid=wd-av-demo-pua-bottom&view=o365-worldwide#use-powershell-cmdlets-to-configure-pua-protection) protection against Potentially Unwanted Apps ([PUA](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/detect-block-potentially-unwanted-apps-microsoft-defender-antivirus?view=o365-worldwide#use-powershell-cmdlets-to-configure-pua-protection))
- [ ] Enable [Bitlocker Encryption with TPM](https://learn.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-device-encryption-overview-windows-10), optionally with [Startup PIN](https://techcommunity.microsoft.com/t5/windows-security/hardening-windows-10-on-an-it-pro-s-laptop/m-p/183213/highlight/true#M232) & read about [Countermeasures](https://learn.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-countermeasures) to reduce [DMA threats](https://support.microsoft.com/en-us/topic/blocking-the-sbp-2-driver-and-thunderbolt-controllers-to-reduce-1394-dma-and-thunderbolt-dma-threats-to-bitlocker-bf0ef10b-f563-5cfc-9740-8340b1d86a0c)
- [ ] Use [Windows Sandbox](https://techcommunity.microsoft.com/t5/windows-kernel-internals-blog/windows-sandbox/ba-p/301849) for new/unknown binaries ([you can use it with the right click menu](https://github.com/damienvanrobaeys/Run-in-Sandbox)) or enable [Hyper-V](https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/about/) for use with Microsoft's [Virtual Machine Platform](https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/quick-create-virtual-machine)
- [ ] Enable [sandboxing](https://www.microsoft.com/en-us/security/blog/2018/10/26/windows-defender-antivirus-can-now-run-in-a-sandbox/) for Microsoft Defender Antivirus
- [ ] [Only elevate executables which are signed and validated](https://docs.microsoft.com/en-us/windows/security/identity-protection/user-account-control/user-account-control-group-policy-and-registry-key-settings#user-account-control-only-elevate-executables-that-are-signed-and-validated)
- [ ] Use the only browser that [natively supports hardware isolation](https://docs.microsoft.com/en-us/deployedge/ms-edge-security-for-business): [Edge](https://www.microsoft.com/en-us/edge)
- [ ] Use [EFS file encryption](https://community.windows.com/en-us/stories/file-encryption-windows-10) for very sensitive files - also compatible with Bitlocker
- [ ] [Harden OneDrive](https://malwaretips.com/threads/hard_configurator-windows-hardening-configurator.66416/page-28#post-743486) with Windows Controlled Folder Access ([CFA](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/controlled-folders?view=o365-worldwide) aka Ransomeware Protection)
- [ ] Avoid old file systems like FAT32 that [do not preserve Alternative NTFS Streams](https://malwaretips.com/threads/how-to-harden-my-system-against-usb-spreading-malware.98442/page-2#post-859762) (where Mark Of The Web is skipped)
- [ ] While DNS encryption [isn't perfect](https://madaidans-insecurities.github.io/encrypted-dns.html) both [Quad9](https://www.quad9.net) and [Cloudflare](https://developers.cloudflare.com/1.1.1.1/setup/) are recommend. [AdGuard](https://adguard-dns.io) and [NextDNS](https://nextdns.io/) are another, but some users report problems like false positive filtering, stability/performance issues.

### :luc_screen_share: Further Hardening


- [ ] [Configure](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/enable-exploit-protection?view=o365-worldwide#windows-security-app) Microsoft's [Exploit Protection](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) and [Enforced CET](https://techcommunity.microsoft.com/t5/windows-kernel-internals/developer-guidance-for-hardware-enforced-stack-protection/ba-p/2163340#toc-hId--1650725290)
- [ ] Use [Microsoft's recommended block rules](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/microsoft-recommended-block-rules)
- [ ] Control [USB devices and other removable media](https://docs.microsoft.com/en-us/windows/security/threat-protection/device-control/control-usb-devices-using-intune)
- [ ] See UEFI Hardening aka [NSA Defensive Practices Guidance](https://www.nsa.gov/Portals/70/documents/what-we-do/cybersecurity/professional-resources/ctr-uefi-defensive-practices-guidance.pdf) and [Hardware-and-Firmware-Security-Guidance](https://github.com/nsacyber/Hardware-and-Firmware-Security-Guidance)
- [ ] See [Hardware and Firmware Security Guidance](https://github.com/nsacyber/Hardware-and-Firmware-Security-Guidance/tree/master/guidance) for [Windows](https://github.com/nsacyber/Hardware-and-Firmware-Security-Guidance/tree/master/guidance#win) and [AMD CPUs](https://github.com/nsacyber/Hardware-and-Firmware-Security-Guidance/tree/master/guidance#54-amd) 
- [ ] Deploy [Windows Security Baselines](https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-security-configuration-framework/windows-security-baselines) and keep it [up-to-date](https://techcommunity.microsoft.com/t5/microsoft-security-baselines/bg-p/Microsoft-Security-Baselines)
- [ ] Use [Mandatory Integrity Control](https://learn.microsoft.com/en-us/windows/win32/secauthz/mandatory-integrity-control)
- [ ] Use [Security-ADMX custom template](https://github.com/Harvester57/Security-ADMX) focused on hardening Windows 10 systems

- HardeningKitty https://github.com/0x6d69636b/windows_hardening

### :luc_check_circle: Get the maximum of defender

The following settings may **decrease the usability of your computer**, since defender will be setup to **shoot everything suspicious** with the help of windows cloud threat intel. It will also, **consume more ressources** !

You can find these settings in the group policy editor under `Computer Configuration > Administrative Templates > Windows Components > Microsoft Defender Antivirus`

> :luc_folder_open: Under the `MAPS` folder :

- [ ] Set `Configure the Block at First Sight` to **"Enabled"**
- [ ] Set `Join Microsoft MAPS` to **"Enabled"** with Options : **"Advanced MAPS"**
- [ ] (As you want) Set `Send file samples when further analysis is required` to **"Enabled"** with Options : **"Send all samples"**

> :luc_folder_open: Under the `MpEngine` folder :

- [ ] Set the [cloud-delivered protection level](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/specify-cloud-protection-level-microsoft-defender-antivirus?view=o365-worldwide#use-group-policy-to-specify-the-level-of-cloud-delivered-protection) to **"Enabled"** with Options : **"Zero Tolerance"** 😵‍💫


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