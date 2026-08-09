# 01 - Microsoft Entra ID Tenant Setup

## Objective

Establish the Microsoft Entra ID environment that will be used throughout the security laboratory.

## Purpose

The tenant provides the identity foundation for the lab.

It will be used to demonstrate:

- User management
- Group management
- Authentication
- Role-Based Access Control
- Conditional Access
- Application identity
- Identity monitoring
- Security investigation

## Lab Design

The environment will use dedicated test identities and resources.

No production identities or production credentials will be used.

## Tenant Configuration

The following configuration will be documented after the tenant is created:

| Configuration | Status |
|---|---|
| Microsoft Entra tenant | Pending |
| Tenant ID | Not documented publicly |
| Custom domain | Not required |
| Security defaults | To be evaluated |
| MFA | To be configured |
| Conditional Access | To be configured |
| Test users | To be created |
| Security groups | To be created |
| Administrative roles | To be configured |
| Audit logging | To be validated |
| Sign-in logging | To be validated |

## Security Principles

The lab will follow:

- Zero Trust
- Least Privilege
- Strong Authentication
- Separation of Administrative Roles
- Continuous Monitoring

## Security Considerations

The following information must never be committed to GitHub:

- Passwords
- Client secrets
- Access tokens
- Refresh tokens
- Private keys
- API keys
- Authentication cookies
- Personal information
- Production credentials

Tenant identifiers may be referenced in private lab notes but should not be unnecessarily exposed in public documentation.

## Validation

The tenant setup will be considered complete when:

- [ ] Tenant is accessible
- [ ] Administrative access is verified
- [ ] Test identity strategy is defined
- [ ] Security configuration is reviewed
- [ ] Logging capabilities are validated

## Next Step

Create the lab users and security groups.
