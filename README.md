# domain-gen

`domain-gen` polls the WHOIS info for domains based on words from a word-list and reports the expiration dates. This is then used to find interesting domain names that may be available for registration.

### Version
0.0.1

### Installation

1. Clone the repository
2. Install the Python-Whois module:
    ```pip install python-whois```
    (see: https://bitbucket.org/richardpenman/pywhois)
3. Run `./generate [word]` to generate a list of domains for that word

A set of default TLDs are queried. To look up specific TLDs, add them using the `-t` flag.
```
# Usage
./generate -t [tld] [word]

# example, looks up domain "foo.bar"
./generate -t bar foo
foo.bar 2020-01-01
```
