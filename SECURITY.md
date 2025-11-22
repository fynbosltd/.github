# Security Policy

## Supported Versions

We take security seriously at Fynbos Ltd. This section describes which versions of our projects are currently supported with security updates.

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |
| < Latest| :x:                |

We generally support security updates for the latest stable release. We encourage all users to keep their installations up to date.

## Reporting a Vulnerability

We appreciate your efforts to responsibly disclose security vulnerabilities. Please follow these guidelines when reporting security issues:

### Where to Report

**DO NOT** create a public GitHub issue for security vulnerabilities.

Instead, please report security vulnerabilities through one of the following channels:

1. **GitHub Security Advisories** (Preferred):
   - Go to the repository's Security tab
   - Click "Report a vulnerability"
   - Fill out the advisory form

2. **Email**:
   - Send details to: security@fynbosltd.com
   - Use PGP encryption if possible (key available upon request)

3. **Private Disclosure**:
   - Contact the maintainers directly through GitHub
   - Mark your message as sensitive/confidential

### What to Include

When reporting a vulnerability, please include:

- **Description**: A clear description of the vulnerability
- **Impact**: The potential impact and severity
- **Reproduction Steps**: Detailed steps to reproduce the issue
- **Affected Versions**: Which versions are affected
- **Proof of Concept**: Code or screenshots demonstrating the issue (if applicable)
- **Suggested Fix**: If you have ideas on how to fix it (optional)
- **Your Contact Information**: So we can follow up with questions

### Example Report

```
Subject: [SECURITY] SQL Injection in User Authentication

Description:
The user authentication endpoint is vulnerable to SQL injection attacks
through the username parameter.

Impact:
An attacker could bypass authentication, access unauthorized data, or
execute arbitrary SQL commands on the database.

Affected Versions:
v1.2.0 through v1.5.3

Steps to Reproduce:
1. Navigate to /login
2. Enter the following in the username field: admin' OR '1'='1
3. Enter any password
4. Click submit
5. Observe successful authentication bypass

Proof of Concept:
[Include code, screenshots, or curl commands here]

Suggested Fix:
Use parameterized queries instead of string concatenation for SQL statements.

Contact: researcher@example.com
```

## Response Timeline

We aim to respond to security reports according to the following timeline:

| Stage | Timeline |
|-------|----------|
| **Initial Response** | Within 48 hours |
| **Vulnerability Confirmation** | Within 1 week |
| **Fix Development** | Varies based on severity |
| **Security Advisory** | Upon fix deployment |
| **Public Disclosure** | 90 days after fix (or earlier if agreed) |

### Severity Levels

We classify vulnerabilities using the following severity levels:

#### Critical
- Remote code execution
- Authentication bypass
- Data breach potential
- **Response**: Immediate action, fix within 24-48 hours

#### High
- Privilege escalation
- SQL injection
- Cross-site scripting (XSS) with significant impact
- **Response**: Fix within 1 week

#### Medium
- Information disclosure
- Denial of service
- CSRF vulnerabilities
- **Response**: Fix within 2-4 weeks

#### Low
- Security configuration issues
- Minor information leaks
- **Response**: Fix in next regular release

## Security Update Process

When a security vulnerability is confirmed:

1. **Acknowledgment**: We acknowledge receipt and confirm the issue
2. **Investigation**: We investigate the scope and impact
3. **Fix Development**: We develop and test a fix
4. **Security Advisory**: We create a security advisory (kept private initially)
5. **Release**: We release a patched version
6. **Notification**: We notify users through:
   - GitHub Security Advisories
   - Email (if registered)
   - Project announcements
7. **Public Disclosure**: We publish the advisory after users have had time to update

## Bug Bounty Program

At this time, we do not offer a paid bug bounty program. However, we deeply appreciate security researchers who help improve our projects:

- Public recognition in our Hall of Fame (with your permission)
- Acknowledgment in security advisories
- Credit in release notes
- Our sincere gratitude 🙏

## Security Best Practices for Users

To keep your installation secure:

1. **Keep Updated**: Always use the latest stable version
2. **Monitor Advisories**: Subscribe to security advisories for our repositories
3. **Follow Documentation**: Implement security recommendations from our docs
4. **Report Issues**: Report any security concerns promptly
5. **Review Dependencies**: Regularly update your dependencies
6. **Use Strong Authentication**: Enable 2FA and use strong passwords
7. **Limit Permissions**: Follow the principle of least privilege

## Security Features

Our projects implement various security features:

- Input validation and sanitization
- Secure authentication mechanisms
- Encrypted data transmission (HTTPS)
- Regular security audits
- Dependency vulnerability scanning
- Security-focused code reviews

## Third-Party Dependencies

We regularly monitor and update our dependencies to address known vulnerabilities. We use automated tools to:

- Scan for vulnerable dependencies
- Receive security alerts
- Update to patched versions promptly

## Compliance

Our projects aim to comply with:

- OWASP Top 10 security risks
- Industry-standard security practices
- Relevant data protection regulations (GDPR, etc.)

## Security Checklist for Contributors

If you're contributing code, please ensure:

- [ ] Input is properly validated and sanitized
- [ ] Authentication and authorization are correctly implemented
- [ ] Sensitive data is encrypted
- [ ] No hardcoded credentials or secrets
- [ ] Dependencies are up to date
- [ ] Security headers are properly configured
- [ ] Error messages don't leak sensitive information
- [ ] Rate limiting is implemented where appropriate

## Hall of Fame

We thank the following security researchers for responsibly disclosing vulnerabilities:

<!-- Add names here with permission -->
- *Be the first to help us improve our security!*

## Questions About Security?

If you have questions about our security practices or policies:

- Review this document thoroughly
- Check our documentation
- Contact us at: security@fynbosltd.com

## Policy Updates

This security policy may be updated periodically. Check back regularly for the latest version.

**Last Updated**: November 22, 2025

---

Thank you for helping keep Fynbos Ltd projects and our users safe! 🛡️
