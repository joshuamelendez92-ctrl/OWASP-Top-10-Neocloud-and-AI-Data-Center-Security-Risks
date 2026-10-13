# OWASP FORGE — Security Glossary

> Draft contribution for review. This document is not an official OWASP publication.

This glossary explains selected security concepts used in the OWASP Top 10 Neocloud and AI Data Center Security Risks (FORGE) framework. Definitions are intended to remain vendor-neutral.

## Attestation

A process of evaluating evidence about a system's identity or security state against trusted reference values or policies. Hardware-backed attestation can use cryptographic measurements to help verify boot integrity, firmware state, or trusted execution environments. Its assurance is limited to the components and properties covered by the verification process.

Related risks: FORGE-01, FORGE-03.

## Baseboard Management Controller (BMC)

A dedicated management processor in a server that provides hardware monitoring and remote administration independently of the host operating system. BMCs commonly support power control, remote console access, firmware updates, and hardware monitoring, making their security critical to infrastructure integrity.

Related risks: FORGE-01, FORGE-04.

## Out-of-Band (OOB) Management

Administration of infrastructure through management interfaces or communication paths independent of the host operating system and typically separated from production networks. OOB management enables remote recovery and configuration, but weak access controls or segmentation can expose privileged infrastructure functions.

Related risk: FORGE-04.

## Tenant Isolation

Security boundaries that prevent customers or workloads sharing infrastructure from accessing or interfering with one another's data, identities, execution environments, and resources. In AI infrastructure, isolation must account for shared accelerators, drivers, storage, networks, and residual data when resources are reassigned.

Related risk: FORGE-03.

## References

- DMTF — Security Protocol and Data Model (SPDM), DSP0274
- Trusted Computing Group — TPM Library Specification
- OpenBMC Project
- DMTF — Redfish specifications
- Kubernetes Documentation — Multi-tenancy
- Confidential Containers Project
