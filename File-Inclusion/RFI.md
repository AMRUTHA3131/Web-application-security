# Remote File Inclusion (RFI)

## Objective

To demonstrate Remote File Inclusion in the controlled DVWA
laboratory.

## Attack Scenario

Remote File Inclusion occurs when an application allows a
user-controlled parameter to reference a remotely located resource.

In a vulnerable configuration, this may allow attacker-controlled
content to be included or executed.

## Demonstration

RFI was tested within the isolated DVWA laboratory environment
using a harmless test file.

## Observation

The application attempted to process the remotely supplied
resource, demonstrating the security risk associated with
unrestricted remote file inclusion.

## Mitigation

- Avoid remote file inclusion functionality when it is not required.
- Use an allowlist of permitted files.
- Validate user-controlled input.
- Disable unnecessary remote URL inclusion.
- Apply least-privilege permissions.

## Testing Environment

- Kali Linux
- DVWA
- Docker
- Local controlled laboratory
