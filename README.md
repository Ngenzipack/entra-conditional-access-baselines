# Entra Conditional Access Baselines

Production-ready baseline Conditional Access policies and rollout guidance for Microsoft Entra ID.

## Overview

This repository defines secure, practical Conditional Access policy baselines to improve identity protection while minimizing operational disruption.

## Problem Being Solved

- Conditional Access rollouts often break user productivity when policies are applied without phased controls.
- Organizations need clear baseline policies aligned to least-privilege and strong authentication.
- Security teams require repeatable documentation for deployment, testing, and exception handling.

## Solution

This project provides baseline policy sets, staged rollout playbooks, and validation checklists for secure Entra deployments.

## Technologies Used

- Microsoft Entra ID (Azure AD)
- Conditional Access
- MFA / Authentication Strengths
- Named Locations / Risk Policies
- PowerShell / Microsoft Graph (planned automation)

## Repository Layout

```text
.
├── baselines/             # Baseline policy definitions
├── rollout-guides/        # Pilot and phased deployment playbooks
├── exceptions/            # Documented exception patterns
├── validation/            # Post-deployment checks and test cases
└── README.md
```

## Setup and Installation

```bash
git clone https://github.com/Ngenzipack/entra-conditional-access-baselines.git
cd entra-conditional-access-baselines
```

Optional management tools:

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
Install-Module Az -Scope CurrentUser
```

## How to Use

1. Review baseline policy set in `baselines/`.
2. Start with pilot users/groups.
3. Validate sign-in behavior and exclusions.
4. Roll out in phases by user segment and workload sensitivity.
5. Track exceptions and remediation timelines.

## Screenshot

![Screenshot Placeholder](./docs/images/screenshot-placeholder.png)

## Key Outcomes / Learnings

- Reduced misconfiguration risk with standardized baseline definitions.
- Faster, safer rollout through phased enforcement patterns.
- Improved consistency between IAM policy intent and user access controls.

## Roadmap

- [ ] Add JSON policy templates for import/export workflows.
- [ ] Add PowerShell automation for policy deployment.
- [ ] Add identity risk and break-glass account reference patterns.

## Contributing

Contributions are welcome. Open an issue for discussion before major changes.

## License

MIT
