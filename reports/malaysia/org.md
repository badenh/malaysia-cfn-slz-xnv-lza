# Coverage report: org

- mapped: 13
- unmapped: 0
- dropped: 0

## Mapped

- lz-organization.json::WorkloadOrganizationalUnit -> organizationalUnits[Workloads]
- lz-organization.json::WorkloadProductionOrganizationalUnit -> organizationalUnits[Production]
- lz-organization.json::WorkloadNonProductionOrganizationalUnit -> organizationalUnits[NonProduction]
- lz-organization.json::InfrastructureOrganizationalUnit -> organizationalUnits[Infrastructure]
- lz-organization.json::ForensicOrganizationalUnit -> organizationalUnits[Forensic]
- lz-organization.json::SandboxOrganizationalUnit -> organizationalUnits[Sandbox]
- lz-organization.json::SuspendedOrganizationalUnit -> organizationalUnits[Suspended]
- lz-organization.json::SecurityOrganizationalUnit -> organizationalUnits[Security]
- lz-organization-scp-guardrails.json::BaselineGuardrailPolicy -> serviceControlPolicies[my-slz-guardrail] targets=['Infrastructure', 'Security', 'Workloads', 'Sandbox', 'Forensic'] (L2-resolved)
- lz-organization-scp-guardrails.json::DeclarativePolicy -> declarativePolicies[EnforceAccountEC2Baseline] targets=['Root'] (L2-resolved)
- lz-organization-scp-approved-services.json::ApprovedServicesPolicy -> serviceControlPolicies[my-slz-approved-services] targets=['Infrastructure', 'Security', 'Workloads', 'Sandbox', 'Forensic'] (L2-resolved)
- lz-organization-rcp-guardrails.json::BaselineResourceGuardrailPolicy -> resourceControlPolicies[my-lza-resource-guardrail] targets=['Infrastructure', 'Security', 'Workloads', 'Sandbox', 'Forensic'] (L2-resolved)
- lz-organization-ai-optout.json::AIServiceOptOutPolicy -> customizations-config.yaml passthrough (Type=AISERVICES_OPT_OUT_POLICY)

## Unmapped (feed to L2)

_(none)_

## Dropped (intentional — engine handles)

_(none)_
