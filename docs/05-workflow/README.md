# ⚙️ 5. Real Workflow Example

[← Framework](../04-framework/README.md) | [Back to Main](../../README.md) | [Next: Benefits →](../06-benefits/README.md)

---

## SOC 2 Type II — Step by Step

```
┌──────────────────────────────────────────────────────────────────────┐
│                    SPRINTO COMPLIANCE WORKFLOW                        │
├──────────────────────────────────────────────────────────────────────┤
│                                                                       │
│  ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐             │
│  │ Step 1  │──▶│ Step 2  │──▶│ Step 3  │──▶│ Step 4  │             │
│  │  Cloud  │   │Security │   │  Risk   │   │Evidence │             │
│  │Integrate│   │  Scan   │   │Detected │   │Collected│             │
│  └─────────┘   └─────────┘   └─────────┘   └─────────┘             │
│                                                   │                  │
│                                                   ▼                  │
│                                          ┌──────────────┐           │
│                                          │   Step 5     │           │
│                                          │  Report Gen  │           │
│                                          └──────────────┘           │
│                                                                       │
│  ┌──────────────────────────────────────────────────────────────┐    │
│  │                   CONTINUOUS MONITORING                       │    │
│  │         (Runs in background throughout the workflow)          │    │
│  └──────────────────────────────────────────────────────────────┘    │
└──────────────────────────────────────────────────────────────────────┘
```

---

## Step 1: Cloud Integration *(30 minutes)*

1. Navigate to Integrations → Add Integration in Sprinto dashboard
2. Select AWS / Azure / GCP and authenticate with read-only credentials
3. Connect Identity Providers (Okta, Google Workspace, or Azure AD)
4. Connect Developer Tools (GitHub, Jira)

**Result**: Sprinto has visibility into your entire tech stack.

---

## Step 2: Security Control Scan *(24–48 hours)*

Sprinto automatically runs checks against **80+ controls**:

| Control Category | Example Checks |
|-----------------|----------------|
| **Authentication** | MFA enabled for all users? |
| **Authorization** | Least privilege permissions? |
| **Encryption** | Data at rest encryption enabled? |
| **Logging** | CloudTrail logging active? |
| **Network** | Security groups properly configured? |
| **Device** | Endpoint protection installed? |

**Compliance Dashboard**:

```
┌─────────────────────────────────────────────────────────────────┐
│                    COMPLIANCE DASHBOARD                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│  Overall Score: ████████████████░░  78%                         │
│                                                                  │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐          │
│  │   PASSING    │  │   WARNING    │  │   FAILING    │          │
│  │      62      │  │      12      │  │       6      │          │
│  └──────────────┘  └──────────────┘  └──────────────┘          │
│                                                                  │
│  ⚠️  MFA not enforced on 3 user accounts                        │
│  ⚠️  AWS S3 bucket 'customer-data' is public                    │
│  ⚠️  CloudTrail logging disabled in us-east-1                   │
└─────────────────────────────────────────────────────────────────┘
```

---

## Step 3: Risk Detection *(Automated, real-time)*

| Severity | Definition | Example |
|----------|------------|---------|
| 🔴 **High** | Immediate security risk | Public S3 bucket, No MFA |
| 🟡 **Medium** | Policy violation | Weak password policy |
| 🟢 **Low** | Best practice gap | Missing security group description |

**Risk Response Flow**:

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│   Detect    │────▶│   Assess    │────▶│  Remediate  │
│    Risk     │     │   Impact    │     │   Issue     │
└─────────────┘     └─────────────┘     └─────────────┘
       │                                       │
       ▼                                       ▼
┌─────────────┐                        ┌─────────────┐
│   Alert     │                        │   Verify    │
│    Team     │                        │    Fix      │
└─────────────┘                        └─────────────┘
```

---

## Step 4: Evidence Collection *(Continuous)*

Sprinto API polls integrated systems hourly, capturing screenshots, logs, and configurations.

```
Evidence ID    Control          Source        Last Collected
──────────────────────────────────────────────────────────────
EV-001        CC6.1 MFA         Okta          2024-01-15 14:32
EV-002        CC6.7 Encryption  AWS KMS       2024-01-15 14:35
EV-003        CC7.2 Logging     CloudTrail    2024-01-15 14:40
```

---

## Step 5: Audit-Ready Report Generation *(Click to generate)*

1. Go to **Reports → SOC 2 Type II → Generate Report**
2. Report includes: executive summary, control matrix, risk assessment, policy docs, vendor results
3. Export as PDF, ZIP, or share via direct auditor portal access

---

## Step 6: Trust Center *(Optional)*

```
┌─────────────────────────────────────────────────────────────────┐
│                    TRUST CENTER PREVIEW                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│  🛡️  SOC 2 Type II Certified   ✓ Annual audit completed         │
│  📜  ISO 27001 Certified        ✓ Cert expires: Dec 2025        │
│  🔒  Security Policies          ✓ Info Security + Privacy       │
│  📊  Security Posture           ✓ MFA: 100% | Enc: AES-256      │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

---

[← Framework](../04-framework/README.md) | [Back to Main](../../README.md) | [Next: Benefits →](../06-benefits/README.md)
