# 0x45dd/tap

Homebrew formulae for [pwner](https://github.com/0x45dd/pwner).

```sh
brew install 0x45dd/tap/pwner
```

Or in a `Brewfile`:

```ruby
tap "0x45dd/tap"
brew "pwner"
```

## Formulae

| Formula | What it is |
|---|---|
| `pwner` | An agentic network pentest tool you talk to — [repo](https://github.com/0x45dd/pwner), [docs](https://www.pwner.si/) |

`pwner` pulls in `nmap`, which is its only hard requirement. The rest of the toolchain it
drives — nuclei, hydra, netexec, impacket and others — is optional and deliberately not
declared here, so installing pwner does not drop a full offensive toolchain onto your
machine. Run `pwner doctor` afterwards to see what is present and how to get the rest.

**Authorized use only.** pwner sends real traffic to the hosts you name and, with your
approval, actively breaks into them. Only run it against systems you own or have explicit,
written permission to test.

## Installing from main

```sh
brew install --HEAD 0x45dd/tap/pwner
```

## License

The formulae here are released under the [BSD 2-Clause license](LICENSE), matching
Homebrew's own. `pwner` itself is AGPL-3.0-or-later; see its repository.
