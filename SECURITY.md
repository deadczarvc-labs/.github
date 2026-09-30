# Security policy

## Supported versions

Only the latest release of each repository receives security fixes.

## Reporting a vulnerability

Please do not open a public issue. Use GitHub private vulnerability reporting instead:

1. Open the **Security** tab of the affected repository.
2. Click **Report a vulnerability**.
3. Describe the problem, the affected version, and the steps to reproduce it.

We aim to acknowledge a report within 7 days. We will keep you informed while we work on a fix, and we will credit you
in the advisory unless you prefer to stay anonymous.

## Scope

These projects process agent transcripts and call external model APIs. Reports we are especially interested in:

- leaks of API keys, tokens or transcript content to logs, files or third parties;
- content sent to an external API that the configuration said would stay local;
- ways for a transcript to make the tool run commands or write files.
