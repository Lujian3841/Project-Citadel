# Security Policy

Project Citadel is documented publicly as a sanitized portfolio project.

## Do Not Commit

- Passwords, tokens, or keys
- Environment files
- VPN private keys or full client profiles
- Database dumps or backup archives
- Private IP addresses or full internal network maps
- Admin-console screenshots that expose sensitive details
- Production configuration files containing live values
- Personal files or screenshots showing private data

## Safe to Document

- High-level architecture
- Technologies used
- Sanitized diagrams
- Sanitized screenshots
- General deployment concepts
- Lessons learned
- Security decisions without sensitive values

## Security Review

If sensitive information is accidentally added, remove it from the public repository and rotate the exposed value in the live environment.
