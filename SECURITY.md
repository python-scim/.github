# Security Policy

This policy applies to every repository of the python-scim organization.

## Reporting a vulnerability

**Please do not open a public issue, pull request or discussion for a security problem.**

Report it privately from the repository of the affected project: open the **Security** tab and
click **Report a vulnerability**. If you are not sure which project is affected, pick the one you
were using, we will move the report if needed.

A useful report includes:

- the affected project and version;
- a description of the problem and why you think it is a security issue;
- a minimal example or the steps to reproduce it;
- the impact you foresee and, if you know one, a mitigation or a fix.

## What happens next

The projects are maintained by a small team, so we cannot guarantee timelines, but we aim to:

- acknowledge the report within 7 days;
- tell you within 30 days whether we consider it a vulnerability, and how we plan to fix it;
- publish a fix and a disclosure within 90 days of the report.

We work on the fix with you in a private security advisory. Once the fixed version is released, we
publish the advisory, request a CVE identifier through GitHub, and credit you unless you prefer not
to be named. Please do not request a CVE yourself, and keep the details private until the advisory
is published.

There is no bug bounty program.

## Supported versions

Security fixes are released for the latest release of each project only. Please check that the
problem still exists with the latest release before reporting it.

## Scope

The following are not considered vulnerabilities, but can be reported as regular issues:

- **Behaviors required by the SCIM RFCs** ([RFC 7643](https://www.rfc-editor.org/rfc/rfc7643),
  [RFC 7644](https://www.rfc-editor.org/rfc/rfc7644)). Hardening options are still welcome.
- **Authentication and authorization in applications.** scim2-models validates and serializes SCIM
  payloads, it does not decide who may read or write a resource.
- **Production deployments of scim2-server.** It is an example server that keeps its resources in
  memory, it is not designed to be exposed to untrusted clients. Problems reachable in its intended
  use, such as a test suite or a local server, are in scope.
- **Changes made by scim2-tester and scim2-cli on the server they target.** Creating, updating and
  deleting resources on that server is what they do. Acting on resources outside of what was asked
  is in scope.
- **Vulnerabilities in dependencies**, unless the way a python-scim project uses the dependency is
  affected. Please report them to the dependency first.
