# RubyGem bootstrap-sass Compromise

bootstrap-sass is a popular Sass version of Bootstrap 3, and counts Diaspora,
and rails_admin among its users. Attackers inserted a backdoor into version
3.2.0.3 and published it to RubyGems. The backdoor was not found on the GitHub
repository itself, so presumably, the attackers did not manage to compromise
the source infrastructure itself. The backdoor installed read the value of a
cookie and evaluated the contents at runtime.

## Impact

The malicious version was uploaded on March 26th, 2019, and the backdoor was
discovered later that same day. RubyGems' downloads page indicates that this
version was downloaded 1,477 times. The Gem was yanked from RubyGems an hour
after the initial report.

## Type of Compromise

It's not entirely clear how the attackers gained write access to be able to
publish a new version of the Gem. The package on RubyGems had two maintainers
who have since rotated their credentials and enabled multi-factor
authentication. The source infrastructure appears to have been unaffected.

## CVE Identifier

- [CVE-2019-10842](https://nvd.nist.gov/vuln/detail/CVE-2019-10842)
