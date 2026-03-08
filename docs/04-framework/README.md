# 🏗️ 4. Sprinto Framework (Full Breakdown)

[← Overview](../03-overview/README.md) | [Back to Main](../../README.md) | [Next: Workflow →](../05-workflow/README.md)

---

## Platform Architecture

Sprinto's platform is built on a layered architecture that handles every aspect of compliance automation:

```
┌───────────────────────────────────────────────────────────────────────┐
│                       SPRINTO PLATFORM LAYER                          │
│                                                                       │
│  ┌─────────────────────────────────────────────────────────────────┐  │
│  │               10-COMPLIANCE FRAMEWORK ENGINE                    │  │
│  │                                                                 │  │
│  │  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐         │  │
│  │  │     Asset     │ │    Access     │ │     Risk      │         │  │
│  │  │  Management   │ │   Control     │ │  Management   │         │  │
│  │  └───────────────┘ └───────────────┘ └───────────────┘         │  │
│  │                                                                 │  │
│  │  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐         │  │
│  │  │    Policy     │ │   Evidence    │ │  Continuous   │         │  │
│  │  │  Management   │ │  Collection   │ │  Monitoring   │         │  │
│  │  └───────────────┘ └───────────────┘ └───────────────┘         │  │
│  │                                                                 │  │
│  │  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐         │  │
│  │  │    Vendor     │ │  Compliance   │ │    Audit      │         │  │
│  │  │  Management   │ │   Mapping     │ │  Management   │         │  │
│  │  └───────────────┘ └───────────────┘ └───────────────┘         │  │
│  │                                                                 │  │
│  │  ┌───────────────┐                                             │  │
│  │  │  Integration  │                                             │  │
│  │  │    Layer      │                                             │  │
│  │  └───────────────┘                                             │  │
│  └─────────────────────────────────────────────────────────────────┘  │
│                                                                       │
│  ┌─────────────────────────────────────────────────────────────────┐  │
│  │                      INTEGRATION LAYER                          │  │
│  │                                                                 │  │
│  │  ┌───────────┐ ┌───────────┐ ┌───────────┐ ┌───────────┐      │  │
│  │  │  Cloud    │ │ IDENTITY  │ │   CODE    │ │    HR     │      │  │
│  │  │ Providers │ │           │ │           │ │           │      │  │
│  │  ├───────────┤ ├───────────┤ ├───────────┤ ├───────────┤      │  │
│  │  │ AWS       │ │ Okta      │ │ GitHub    │ │ BambooHR  │      │  │
│  │  │ Azure     │ │ Google WS │ │ GitLab    │ │ Workday   │      │  │
│  │  │ GCP       │ │ Azure AD  │ │ Bitbucket │ │ Gusto     │      │  │
│  │  └───────────┘ └───────────┘ └───────────┘ └───────────┘      │  │
│  │                                                                 │  │
│  │  ┌───────────┐ ┌───────────────────────────────────────────┐   │  │
│  │  │  COMMS    │ │          + 200 more integrations           │   │  │
│  │  ├───────────┤ └───────────────────────────────────────────┘   │  │
│  │  │ Slack     │                                                  │  │
│  │  │ MS Teams  │                                                  │  │
│  │  │ Jira      │                                                  │  │
│  │  └───────────┘                                                  │  │
│  └─────────────────────────────────────────────────────────────────┘  │
└───────────────────────────────────────────────────────────────────────┘
```

---

## 10 Core Components

| # | Component | Details |
|---|-----------|---------|
| 4.1 | [Asset Management](./4.1-asset-management.md) | Discover & track all tech assets |
| 4.2 | [Access Control](./4.2-access-control.md) | Manage identities & permissions |
| 4.3 | [Risk Management](./4.3-risk-management.md) | Identify, assess & mitigate risks |
| 4.4 | [Policy Management](./4.4-policy-management.md) | 100+ auditor-approved templates |
| 4.5 | [Evidence Collection](./4.5-evidence-collection.md) | Automated API-driven collection |
| 4.6 | [Continuous Monitoring](./4.6-continuous-monitoring.md) | Always-on real-time checks |
| 4.7 | [Vendor Management](./4.7-vendor-management.md) | Third-party risk tracking |
| 4.8 | [Compliance Mapping](./4.8-compliance-mapping.md) | Cross-framework control mapping |
| 4.9 | [Audit Management](./4.9-audit-management.md) | Collaborative auditor workspace |
| 4.10 | [Integration Layer](./4.10-integration-layer.md) | 200+ system connections |

---

[← Overview](../03-overview/README.md) | [Back to Main](../../README.md) | [Next: Workflow →](../05-workflow/README.md)
