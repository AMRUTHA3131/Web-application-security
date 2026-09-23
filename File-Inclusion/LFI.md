# Local File Inclusion (LFI)

## Objective

To demonstrate Local File Inclusion in DVWA using a controlled
laboratory environment.

## Attack Scenario

Local File Inclusion occurs when an application uses
user-controlled input to determine which local file should be
included or read.

If the application does not properly validate the supplied file
path, an attacker may attempt to access unintended local files.

## Demonstration

LFI was tested against the DVWA File Inclusion functionality.

A local file path was supplied through the vulnerable parameter
within the isolated laboratory.

## Observation

The application attempted to process the supplied file path,
demonstrating the risk associated with user-controlled file
inclusion.

## Mitigation

- Use an allowlist of permitted files.
- Validate file names and paths.
- Avoid user-controlled file paths.
- Normalize and validate file paths.
- Apply least-privilege permissions.

## Testing Environment

- Kali Linux
- DVWA
- Docker
- Localhost
