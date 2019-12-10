# Webmin backdoor

Webmin, a web-based configuration tool for system administration
for Unix-like systems, was backdoored. The malicous code would
allow attackers execute commands as root.

## Impact

The vendor's build infrastructure was compromised in April 2018,
and the zero day exploit was discovered in August 2019.
Users who downloaded the backdoored version in between
might have been affected. It is notable that the compromise
did not affect any GitHub repository, and therfore,
any user who built their own copy of Webmin from GitHub is being safe.

## Type of Compromise

The Webmin development build server was exploited and a
vulnerability was added to the Webmin source code.
The attacker didn't compromise any key, but rather just the infrastructure.

## CVE Identifier

- [CVE-2019-15107](https://nvd.nist.gov/vuln/detail/CVE-2019-15107), [CVE-2019-15231](https://www.cvedetails.com/cve/CVE-2019-15231/)
