# Lab 01 — Microsoft Entra ID & Conditional Access

## Objective

Configure and validate a Microsoft Entra Conditional Access policy requiring multifactor authentication (MFA) for a designated lab user.

This lab demonstrates the implementation, testing, and validation of an identity security control using Microsoft Entra ID.

---

## Environment

- Microsoft Azure
- Microsoft Entra ID
- Microsoft Entra ID P1
- Microsoft Entra Conditional Access
- Microsoft Entra users and groups

---

## Lab Scenario

A simulated organization wants to strengthen identity security by requiring MFA for designated users.

The goal of this lab was to create test identities, configure the required licensing, create a Conditional Access policy, safely test the policy, and validate the final enforcement state.

---

## Implementation

### 1. Created Lab Users

Created dedicated test identities for the lab:

- `labuser01`
- `labuser02`

These accounts were used to test the Conditional Access configuration without affecting unrelated users.

---

### 2. Created Conditional Access Security Group

Created a dedicated security group:

`CA-Lab-Users`

The group was used to scope the Conditional Access testing to the designated lab users.

---

### 3. Configured Microsoft Entra ID P1

Microsoft Entra ID P1 was activated and assigned to the lab administrator.

This provided the licensing required to configure Conditional Access policies.

---

### 4. Created Conditional Access Policy

Created the following Conditional Access policy:

`MFA for Lab Users`

The policy was configured to require multifactor authentication for the designated lab user.

---

### 5. Tested the Policy

The policy was initially configured in:

**Report-only**

Report-only mode allowed the configuration to be evaluated without immediately enforcing the policy.

This provided a safer way to validate the configuration before enabling enforcement.

---

### 6. Enabled the Policy

After reviewing the configuration, the policy was enabled.

Final policy state:

**On**

The policy requires MFA for the designated lab user.

---

## Security Controls Demonstrated

- Microsoft Entra ID user management
- Security group management
- Microsoft Entra ID P1 licensing
- Conditional Access
- Multifactor Authentication (MFA)
- Report-only policy testing
- Identity security policy enforcement

---

## Evidence

Screenshots documenting the lab configuration and validation are stored in the `screenshots` directory.

Evidence includes:

1. Lab users created
2. Conditional Access security group
3. Microsoft Entra ID P1 license assignment
4. Conditional Access policy creation
5. Policy configuration and testing
6. Final policy validation

---

## Lessons Learned

This lab demonstrated how Conditional Access can be used to enforce identity security controls based on users, groups, applications, and authentication requirements.

Using Report-only mode before enforcement provides a safer method for testing Conditional Access policies and reducing the risk of unintended access disruption.

---

## Result

The **MFA for Lab Users** Conditional Access policy was successfully configured, tested, and enabled.

**Status: Completed**
