# CVSS v3.1 Base Score Assessment

## Base Metric Justification

### Attack Vector — Local (AV:L)

The vulnerability is scored as Local because the vulnerable component is not bound to the network and the attacker's path is read/write/execute. So, according to "FIRST", if the attacker exploits the vulnerability by accessing the system locally (e.g keystrokes), remotely (via SSH), or if the attacker relies on User Interaction by another person to perform actions required to exploit the vulnerability (e.g tricking a legitimate user into opening a malicious document), then the attack vector is considered Local.

### Attack Complexity — Low (AC:L)

The attack complexity is rated Low because the attacker can expect repeatable success against the vulnerable component. And successful attack does not depend on conditions beyond attacker's control.

A specially crafted PDF can trigger the buffer overflow when processed by a vulnerable version of Adobe Acrobat or Reader. The exploitation scenario does not depend on a race condition or other highly specialised circumstances.

### Privileges Required — None (PR:N)

No special privileges are required to exploit the vulnerability. 

The attacker also does not need an existing account or elevated permissions on the target system. The attack instead relies on getting a malicious document to the victim and convincing the victim to open it.

### User Interaction — Required (UI:R)

User Interaction is Required because the victim must open the malicious PDF for exploitation to occur.

This is a significant part of the attack chain. Simply delivering the malicious document to the victim is not sufficient; the vulnerable application must process the document.

The attacker won't be able to exploit the vulnerability if the user does not open the file. 

### Scope — Unchanged (S:U)

The Scope is Unchanged because exploitation affects the same security authority as the vulnerable component.

The vulnerable Adobe application and the resulting impact are considered within the same security authority of the affected system. Therefore, exploitation does not cross into a separate security authority.

In other words, the attacker cannot gain access to resources that are outside the security authority of the compromised application.

### Confidentiality — High (C:H)

A successful exploit can result in arbitrary code execution on the affected system.

This can allow an attacker to access information available to the compromised process and potentially the underlying user account. Under the worst-case scenario used by the CVSS assessment, this represents a High Confidentiality impact.

### Integrity — High (I:H)

Successful arbitrary code execution can allow an attacker to modify data, applications, or system settings available to the compromised account.

Under the worst-case scenario, an attacker could gain sufficient control to make significant unauthorised changes to the affected system. Therefore, the Integrity impact is assessed as High.

### Availability — High (A:H)

Successful exploitation can also compromise the availability of the affected system.

An attacker who achieves arbitrary code execution could disrupt services, terminate processes, modify system components, or otherwise interfere with the normal operation of the host. Under the CVSS worst-case assessment, this represents a High Availability impact.

## Base Score

The selected metrics produce the following CVSS v3.1 vector:

CVSS:3.1/AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H

Base Score: 7.8 (High)

The score reflects the combination of a relatively straightforward exploitation path with required user interaction and potentially severe impacts to confidentiality, integrity, and availability.

## Conclusion

The Base Score establishes the intrinsic severity of CVE-2009-0658. It indicates that, although exploitation requires user interaction and occurs through a locally processed malicious document, successful exploitation can have severe consequences because arbitrary code execution may result in high impacts to confidentiality, integrity, and availability.

The Base Score will therefore be used as the foundation for the Temporal Score and Environmental Score assessments in the following stages of this project.
