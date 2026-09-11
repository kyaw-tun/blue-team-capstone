# CVSS v3.1 Environmental Score Assessment

## Environmental Metrics Justification

### Confidentiality Requirement — High (CR:H)

The organization's workstations handle highly sensitive corporate documents and data. Unauthorized access to this information could have a significant impact on the organization.

### Integrity Requirement — High (IR:H)

The integrity of the organization's systems and data is critical. A compromised workstation could also be used to affect other systems on the network.

### Availability Requirement — Medium (AR:M)

Loss of an individual workstation would disrupt the user's work, but would not directly affect core infrastructure or overall business continuity.

## Environmental Score

No Modified Base or Temporal metrics were applied. The assessment assumes standard corporate endpoints without additional security controls, such as sandboxing, that would reduce the potential impact of the vulnerability.

The selected metrics produce the following CVSS v3.1 vector:

`CVSS:3.1/AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H/E:H/RL:O/RC:C/CR:H/IR:H/AR:M`

Environmental Score: 7.5 (High)

## Conclusion

The Environmental Score reflects the importance of confidentiality, integrity, and availability within the fictional organization. High Confidentiality and Integrity Requirements increase the potential impact of a successful compromise, while the Medium Availability Requirement reflects the more limited impact of losing an individual workstation.
