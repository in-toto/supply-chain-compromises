# strong_password RubyGem Breach

The account of the developer of the strong_password RubyGem was hijacked by
unknown attackers. They released a backdoored version of the Gem which
ran arbitrary code stored on pastebin.com if the Gem was running in a
production environment. The Gem also sent a request to the attacker's
server to store the URLs of infected hosts.

## Impact

The backdoor was detected in July 2019, and the last legitimate version of the
Gem was six months prior. Users who installed the Gem in that time frame could
have been affected.

## Type of Compromise

The account used by the developer to publish the Gem was hijacked. The source
infrastructure itself was unaffected. The developer suspects it was due to
their use of an unsafe password and the lack of multi-factor authentication.

## CVE Identifier

- [CVE-2019-13354](https://nvd.nist.gov/vuln/detail/CVE-2019-13354)
