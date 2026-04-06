# Active-Directory-Attack-Investigation
incident response investigation into a critical breach at EmberForge Studios, where unreleased game source code was leaked to underground forums.

EmberForge: Source Leak = Active Directory Attack Investigation

This project documents a full incident response investigation into a critical breach at EmberForge Studios, where unreleased game source code was leaked to underground forums.

The analysis traces the attacker’s activity across a 3-host Windows domain environment (Workstation → Server → Domain Controller) using Sysmon and Windows Security logs in Microsoft Sentinel. The investigation follows the MITRE ATT&CK kill chain, covering initial access, execution, lateral movement, persistence, and data exfiltration.

Key findings include:

Credential access via NTDS.dit extraction using Volume Shadow Copy
Lateral movement using SMB and remote execution
Persistence through scheduled tasks and remote access tools (AnyDesk)
Data exfiltration using cloud sync tooling (rclone)

📄 A detailed report is attached, outlining:

Full attack timeline
Techniques and tools used
Detection gaps and recommendations
