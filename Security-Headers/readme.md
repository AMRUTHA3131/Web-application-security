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

```bash
curl -I http://127.0.0.1
