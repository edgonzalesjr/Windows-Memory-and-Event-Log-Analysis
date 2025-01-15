## Objective

Effectively use Volatility for Windows Memory Analysis and DeepBlueCLI for Windows Event Log Analysis.

### Skills Learned

- Windows Memory Analysis
  - Grasp the significance of volatile memory in forensic investigations, especially for malware detection.
  - Import and analyze memory dumps to generate process lists and pinpoint suspicious processes.
  - Perform advanced memory analysis to identify process injection, malware behaviors, and network activity associated with malicious actions.
- Windows Event Log Analysis:
  - Utilize Windows Event Viewer to collect and interpret forensic data from logs, focusing on user account changes, privilege escalations, and password spraying attacks.
  - Detect and analyze encoded PowerShell commands and evasion tactics.
  - Apply DeepBlueCLI for advanced detection techniques, including PowerShell encoding and detailed EVTX file analysis.

### Tools Used

- Volatility: an open-source framework for extracting digital artefacts from volatile memory (RAM) samples.
- DeepBlueCLI: a Powershell module for Threat Hunting via Windows Event Logs.

## Practical Exercises

- Volatility
<p align="center">
<img src="https://i.imgur.com/tzmfVeW.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://i.imgur.com/ors8StP.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Generate a process list to identify active processes. Suspicious processes like "TrustMe.exe" found.</b>
<br/>

<p align="center">
<img src="https://i.imgur.com/XaSPGAJ.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://i.imgur.com/Ux0TegW.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Detects signs of process injection and malware behavior in memory. Identified suspicious patterns in system processes (e.g., TrustMe.exe).</b>
<br/>

<p align="center">
<img src="https://i.imgur.com/odup4zI.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://i.imgur.com/Yl56j8a.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Lists all network connections to identify suspicious activity (e.g., TrustMe.exe).</b>
<br/>

<p align="center">
<img src="https://i.imgur.com/F8aKXmY.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>List all the DLLs loaded by the process with PID 5452.</b>
<br/>

- DeepBlueCLI
<p align="center">
<img src="https://i.imgur.com/pQAawZp.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Detecting User Account Changes. Adding users for persistence. Event ID 4732 shows a user added to the local administrators group.</b>
<br/>

<p align="center">
<img src="https://i.imgur.com/qYZww1j.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Password Spraying Attacks. Using a list of users with a single password to evade account lockout. Effective because it avoids triggering lockout policies.</b>
<br/>

<p align="center">
<img src="https://i.imgur.com/PgHdUYQ.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://i.imgur.com/AFAQ3cS.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Powershell Encoding Detection. Attackers use encoding to bypass detection.</b>
<br/>

## Outcome

- Achieved proficiency in using both Volatility and Deep Blue CLI for a comprehensive approach to Windows forensic analysis. This includes analyzing memory dumps and event logs to detect and investigate suspicious activities, identify malware behaviors, and effectively respond to security incidents.

## Acknowledgements
- [Volatility](https://volatilityfoundation.org/)
- [DeepBlueCLI](https://www.sans.org/tools/deepbluecli/)

## Disclaimer

The sole goals of the projects and activities here are for education and ethical cybersecurity research. All work was conducted in controlled environments, such as paid cloud spaces, private labs, and online cybersecurity education platforms. Online learning and cloud tasks adhered closely to all usage guidelines. Never use these projects for improper or unlawful purposes. It is always prohibited to break into any computer system or network. Any misuse of the provided information or code is not the responsibility of the author or authors. 
