# Web Security Headers

## Objective

To inspect HTTP security headers and understand their role in
protecting web applications.

## Attack Scenario

Missing or incorrectly configured HTTP security headers can
increase exposure to attacks such as clickjacking, MIME-type
confusion and certain XSS-related attacks.

## Demonstration

HTTP response headers were inspected using:

```bash```
```curl -I http://127.0.0.1```  

The response was examined for security-related headers.

## Headers Observed

#### Examples include:

- X-Content-Type-Options
- X-Frame-Options
- Referrer-Policy
- Mitigation

Appropriate HTTP security headers should be configured according
to the application's requirements.

#### Important headers include:

- Content-Security-Policy
- X-Content-Type-Options
- X-Frame-Options
- Referrer-Policy
- Strict-Transport-Security

## Observation

Security headers provide additional browser-side protections and
help reduce the impact of several web application security risks.

## Testing Environment
- Kali Linux
- Local web application
- Apache
