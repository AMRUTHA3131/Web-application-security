
# Cross-Site Scripting (XSS)

## Objective

To demonstrate Stored XSS and Reflected XSS in the DVWA
application.

## Attack Scenario

Cross-Site Scripting occurs when an application processes
user-controlled input and allows it to be interpreted as
JavaScript in a user's browser.

## 1.Stored XSS

A harmless JavaScript test payload was entered into the DVWA
Stored XSS functionality.

### Test Payload

### html
```<script>alert('XSS')</script>```
The JavaScript alert was executed when the stored content was
displayed.

## 2.Reflected XSS

A harmless XSS payload was supplied through a query parameter.

### Test Payload
```<script>alert('XSS')</script>```

The payload was reflected by the application and executed in the
browser.

## Observation

The JavaScript alert demonstrated that user-controlled input was
being interpreted as JavaScript.

## Mitigation
1. Input Validation

Validate user input according to the expected format and reject
unexpected input.

2. Output Encoding

Encode untrusted data before displaying it in an HTML response.

3. Content Security Policy

Implement an appropriate Content Security Policy (CSP) to restrict
the execution and loading of scripts.

## Testing Environment
- Kali Linux
- DVWA
- Docker
- Localhost
