# CVSS v3.1 Environmental Score Assessment

## Environmental Metrics Justification

### Confidentiality Requirement — High (CR:H)

The organization's workstations handle highly sensitive corporate documents and data. Preventing unauthorized access to this information is therefore critical to the organization.

### Integrity Requirement — High (IR:H)

Protecting the integrity of the organization's systems and data is essential. Preventing malware installation and unauthorized modifications to endpoints is particularly important because compromised workstations could be used to affect the wider network.

### Availability Requirement - Medium (AR:M)

A compromised or unavailable individual workstation would disrupt the productivity of its user. However, the impact would not directly threaten core network infrastructure or overall business continuity, so the Availability Requirement is assessed as Medium.

## Environmental Score

No Modified Base or Temporal metrics were applied. The assessment assumes standard corporate endpoints without additional security controls, such as sandboxing, that would reduce the potential impact of the vulnerability.

The selected metrics produce the following CVSS v3.1 vector:

CVSS:3.1/AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H/E:H/RL:O/RC:C/CR:H/IR:H/AR:M

Environmental Score: 7.5

## Conclusion

The Environmental Score reflects the importance of confidentiality, integrity, and availability within the fictional organization. The high Confidentiality and Integrity Requirements indicate that successful exploitation could have a significant effect on the organization, while the Medium Availability Requirement reflects the more limited impact of losing an individual workstation.
