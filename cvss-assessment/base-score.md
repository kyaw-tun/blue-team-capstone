# CVSS v3.1 Base Score Assessment

## Base Metric Justification

### Attack Vector — Local (AV:L)

The vulnerability is triggered when a malicious PDF is processed locally by a vulnerable version of Adobe Acrobat or Reader. The attack therefore requires the vulnerable application to process the malicious document on the target system.

### Attack Complexity — Low (AC:L)

Exploitation does not require a race condition or other uncommon circumstances. A specially crafted PDF can trigger the vulnerability when processed by the affected application.

### Privileges Required — None (PR:N)

The attacker does not need an account or existing privileges on the target system. The attack relies on getting the malicious document to the victim.

### User Interaction — Required (UI:R)

The victim must open the malicious PDF for the vulnerability to be triggered. Without this interaction, exploitation does not occur.

### Scope — Unchanged (S:U)

The exploitation and resulting impact remain within the same security authority as the vulnerable application. The attack does not cross into a separate security authority.

### Confidentiality — High (C:H)

Successful exploitation can result in arbitrary code execution, allowing an attacker to access sensitive information available to the compromised process or user.

### Integrity — High (I:H)

Successful exploitation can allow an attacker to modify data, applications, or system settings available to the compromised account.

### Availability — High (A:H)

Successful exploitation can allow an attacker to disrupt processes, modify system components, or otherwise interfere with the normal operation of the affected system.

## Base Score

The selected metrics produce the following CVSS v3.1 vector:

`CVSS:3.1/AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H`

Base Score: 7.8 (High)

The score reflects the combination of a relatively straightforward exploitation path with required user interaction and potentially severe impacts to confidentiality, integrity, and availability.

## Conclusion

The Base Score establishes the intrinsic severity of CVE-2009-0658. It indicates that, although exploitation requires user interaction and occurs through a locally processed malicious document, successful exploitation can have severe consequences because arbitrary code execution may result in high impacts to confidentiality, integrity, and availability.

The Base Score will therefore be used as the foundation for the Temporal Score and Environmental Score assessments in the following stages of this project.
