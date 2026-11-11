# Claude Burp Suite Testing Skill

A web application security testing skill for using Burp Suite to inspect, intercept, replay, and assess HTTP traffic within an authorized testing scope.

## What It Covers

- **Proxy setup:** Configure the Burp proxy and browser for HTTP and HTTPS testing.
- **Traffic inspection:** Intercept requests and review HTTP history and site maps.
- **Request modification:** Safely test application behavior by modifying requests in a controlled environment.
- **Repeater:** Replay requests with changed inputs and compare server responses.
- **Target scope:** Define in-scope hosts to reduce noise and prevent unintended testing.
- **Automated scanning:** Review scanner workflows available in Burp Suite Professional.
- **Intruder:** Understand payload positions and attack types for authorized, controlled validation.
- **Reporting:** Record evidence, findings, limitations, and remediation advice.

## Installation and Setup

Clone the repository into your Claude skills directory:

```bash
git clone https://github.com/Brajesh31/claude-burp-suite-testing-skill.git ~/.claude/skills/burp-suite-testing
```

Install and launch Burp Suite using the official PortSwigger documentation. Configure the browser to use the local proxy listener and install the Burp CA certificate only in a dedicated testing browser or environment.

## Using the Skill

Example request:

```text
Use the burp-suite-testing skill to inspect authentication requests
and assess session security in my authorized staging application.
```

Read [SKILL.md](SKILL.md) for the detailed workflow, Burp features, example request analysis, constraints, and troubleshooting steps.

## Authorization and Scope

Use Burp Suite only against applications you own or have explicit written permission to test. Define target scope before active testing, use dedicated test accounts, follow agreed rate limits, and avoid real users' credentials or data. Do not run brute-force, credential stuffing, or disruptive scans outside an explicitly authorized test plan.

## Edition Differences

Burp Suite Community and Professional provide different feature sets. The skill notes that automated scanning and full Intruder capabilities require Professional, while core Proxy and Repeater workflows are available in Community.
