# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.1] — 2026-03-25

### Added
- IT role mining using bottom-up methodology against PROD AD application
- Role mining results analysis with entitlement cluster matrix across identity groups
- IT roles created from discovered entitlement patterns (bottom-up)
- Business roles designed from departmental access requirements (top-down)
- Birthright roles for automatic day-one access assignment based on department and employeeType
- Manager Certification campaigns for manager-to-direct-report access reviews
- Entitlement Owner Certification campaigns for entitlement-level access reviews
- New screenshots: role mining configuration (Figure 7A), role mining results (Figure 7B), certifications (Figure 11A)

### Changed
- Expanded implementation documentation with structured subsections for role mining, role design, lifecycle, and certifications
- Enhanced Figure 9C (birthright role assignment) and Figure 10 (IT/business role structure) descriptions
- Updated README with Role Mining & Role Design and Access Governance & Certification sections
- Updated skills table with role mining, IT/business role design, birthright provisioning, certification campaigns, and compliance readiness
- Moved certification campaigns from planned (v1.1) to completed (v1.0) in the roadmap

## [1.0.0] — 2026-03-25

### Added
- Active Directory as the on-prem identity source with structured OU hierarchy and governance attributes
- SailPoint IdentityIQ as the identity governance platform with Java and Apache Tomcat runtime
- AD connector configuration, identity aggregation, and provisioning integration
- Identity attribute mapping for governance-driven automation
- Joiner, Mover, and Leaver lifecycle event design and business process workflows
- Business roles aligned to departments with birthright-style access
- Workgroup ownership and delegated governance structure
- AD Connect / Microsoft Entra Connect for hybrid identity synchronisation
- Synced users and groups visible in Microsoft Entra ID
- LDAP, LDAPS, certificate, and Java truststore troubleshooting documentation
- SailPoint connector and IQService debugging documentation
- Tomcat runtime and HTTP 405 investigation documentation
- End-to-end access request, approval, provisioning, and AD group membership validation
- Comprehensive screenshots and architecture diagrams
- Full documentation suite (architecture, implementation, troubleshooting, validation, lessons learned)

### Infrastructure
- VMware-based multi-VM lab environment
- Dedicated VMs for AD, SailPoint IIQ, and AD Connect
- Microsoft Entra ID tenant for cloud identity layer

[1.0.1]: https://github.com/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project/releases/tag/v1.0.0
