# Implementation

## Environment Build

The lab was built on a VM-based setup to reflect a real enterprise IAM environment.

## Runtime Foundation

- Active Directory hosted on Windows Server VM
- SailPoint IdentityIQ hosted on dedicated VM
- Java and Apache Tomcat installed locally on IIQ server
- AD Connect hosted on separate VM

## SailPoint Build Areas

### Connector and Aggregation
- Active Directory application onboarding
- Connector validation and IQService support
- Account aggregation and identity correlation
- Identity attribute mapping

### Role Mining and Role Design
- IT role mining using bottom-up methodology against the PROD AD application
- Mining scope filtered by population and entitlement exclusions to surface meaningful patterns
- Entitlement cluster analysis across identity groups to identify candidate roles
- IT roles created from discovered entitlement patterns (bottom-up)
- Business roles designed from departmental access requirements (top-down)
- Birthright roles defined for automatic assignment to new joiners based on `department` and `employeeType`
- Separation between IT roles (technical entitlement bundles) and business roles (job-function access)

### Lifecycle Automation
- Lifecycle event creation for Joiner, Mover, and Leaver
- Business process configuration for JML workflows
- Birthright role assignment triggered automatically through the Joiner workflow
- Attribute-driven access logic using `department` and `employeeType`

### Access Governance
- Workgroups and ownership for delegated governance
- Business roles and governed access structure
- Controlled access request and provisioning process

### Certification Campaigns
- Manager Certification campaigns configured for manager-to-direct-report access reviews
- Entitlement Owner Certification campaigns configured for entitlement-level access reviews
- Multiple campaign executions demonstrating repeatable certification scheduling
- Certification coverage supports SOX and ISO 27001 compliance readiness

## Hybrid Identity Build Areas
- AD Connect installation and sync configuration
- Synced users and groups visible in Entra ID
- Entra Connect health monitoring and validation

## Result

The implementation produced a working IAM model covering identity governance, role mining, IT and business role design, birthright provisioning, certification campaigns, JML automation, hybrid sync, server runtime support, and target-system provisioning validation.
