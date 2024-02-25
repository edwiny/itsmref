# Identity management concepts


## Identity

A collection of unique identifiers or attributes that represent a human, workload, or device.

Three broad types:

* Human: employees, contractors
* Workload identiies: application, service, script, batch process
* Device identities: laptops, phones, servers

## Authentication (aka AuthN)

The process of challenging an actor (human, machine, device) for  **credentials**.

Credentials can be:
* something they know, e.g. password
* something they have, e.g. yubikey, security token, badge, certificate
* something they are, e.g. fingerprint, face, mac address

## SSO

Allow user to do authentication once with an identity provider, then silently authenticate 
when accessing other services. The identity provider becomes a trusted source of identity information,
vouching for the user.


## Authorizatin (AuthZ)

The access control list of what resources the identity has access to.

## PAM

Sudo-as-a-service. Contains and manages all privileged access by people or systems.


## MSI

Managed service identity.
Temporary identity associated with a compute node that allows scripts on that compute node
to authenticate against other services without the need for credentials or passwords.


## SCIM

System for Cross Domain Identity Management

A JSON API used to provision users (identities) into various systems. It enables:

* Automatic provisioning of new accounts
* Automatic deprovisioning
* Synchronizing data between systems
* Group provisioning - whole groups of employees can be given access to the apps that they need.
* Governing access - SCIM makes it easier to monitor and audit privileges.

More info: https://www.microsoft.com/en-us/security/business/security-101/what-is-scim


## Security Assertions

Statements that service providers use to decide whether to grant access to a resource. 

## SAML

Security Assertion Markup Language

Standard protocol to provide security assertions to service providers.
When SAML authenticates that your identity can have access to a resource, it gives you an access token for a single session in your browser