# Security Policy

## Supported Versions

| Version | Supported |
| ------- | --------- |
| 1.x     | ✅ Yes     |
| 0.x     | ❌ No      |

## Reporting a Vulnerability

We take the security of this project seriously. If you discover a security vulnerability, please report it responsibly.

### How to Report

**Do not** open a public issue for security vulnerabilities.

Instead, please report security issues via one of the following methods:

1. **GitHub Security Advisory** (Preferred)
   - Go to the [Security tab](https://github.com/aanirids-glitch/test-repo/security) in the repository.
   - Click on "Report a vulnerability" and fill out the form.

2. **Email**
   - Send details to: `security@aanirids.dev` (or your preferred contact email)
   - Include "SECURITY" in the subject line.

### What to Include

When reporting a vulnerability, please provide:

- A description of the vulnerability.
- Steps to reproduce the issue.
- Potential impact of the vulnerability.
- Any suggested mitigations or fixes (if available).

## Response Timeline

- We will acknowledge receipt of your report within **24 hours**.
- We will provide a preliminary assessment within **72 hours**.
- We will keep you informed of the progress towards a fix.

## Security Best Practices

### For Developers

- **Never commit secrets**: API keys, tokens, passwords, etc. Use environment variables.
- **Validate all inputs**: Sanitize and validate user inputs on both client and server.
- **Use HTTPS**: Ensure all network traffic is encrypted.
- **Keep dependencies updated**: Regularly update dependencies to patch known vulnerabilities.
- **Use security headers**: Implement appropriate security headers (CSP, X-Frame-Options, etc.).

### For the Project

- **Dependency Scanning**: This project should use GitHub's Dependabot or similar tools to scan for vulnerable dependencies.
- **Security Audits**: Periodic security audits are recommended.
- **Code Reviews**: All pull requests should be reviewed for security implications.

## Known Security Considerations

- **Environment Variables**: Never expose sensitive environment variables to the client-side. Prefix public variables with `VITE_` only if necessary.
- **Cross-Site Scripting (XSS)**: Be cautious when rendering user-generated content. Use `dangerouslySetInnerHTML` only when absolutely necessary and with proper sanitization.
- **Cross-Site Request Forgery (CSRF)**: Implement CSRF tokens for state-changing operations.

## Contact

For any questions about this security policy, please contact the maintainers.

---

*This security policy is adapted from the [GitHub Security Policy](https://docs.github.com/en/site-policy/security-policies/github-security-policy).