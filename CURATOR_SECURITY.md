# Security guidance

Use synthetic data and a dedicated development environment. Never commit tokens,
private tenant identifiers, client secrets, certificates, customer data, or .env files.
Prefer managed identity in Azure and interactive delegated login locally. Grant only
the permissions required by each operation; review admin consent and connector scopes.
Keep credentials in an OS credential store or Azure Key Vault. Do not print access tokens.
Validate webhook authenticity, payload sizes, and untrusted input before processing.
Use idempotency, bounded retries, audit logging without personal data, and least privilege.
Deployment is manual; cloud resources and premium connectors may incur charges.

Report vulnerabilities privately through GitHub private vulnerability reporting when
enabled. Do not disclose credentials in public issues. Rotate accidentally exposed secrets
immediately; deleting a file does not remove it from history.

## Dependency audit snapshot

GitHub reported 0 open dependency alerts on 2026-09-15.
Severity counts: `{}`.
These counts cover the upstream sample collection and are not proof that every sample is exploitable.
Review alerts for the selected sample, remediate dependencies, and test before execution.
Fork workflows remain disabled. Secret-scanning results are a point-in-time check, not a complete security audit.
