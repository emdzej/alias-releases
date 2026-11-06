# ALIAS releases

The public packages for using and integrating [ALIAS](https://getalias.support) (Anonymous, Live,
In-context Assistance Service): the clients your product embeds, the command-line tools, and the API's
specification. Everything here is under the MIT licence.

The server isn't here. Use the [hosted service](https://getalias.support/pricing), or ask about a
self-hosted licence: [contact us](https://emdzej.pl).

## Clients

| | |
|---|---|
| **TypeScript** (browser, Node) | `npm install alias-support` |
| **Swift** (iOS, macOS) | [alias-client-swift](https://github.com/emdzej/alias-client-swift): `.package(url: "https://github.com/emdzej/alias-client-swift", from: "X.Y.Z")`, then `AliasSupport` and `AliasSupportUI` |
| **Godot 4** | [alias-client-godot](https://github.com/emdzej/alias-client-godot) (a tag per release), or `alias-support-godot_X.Y.Z.zip` on each [release](https://github.com/emdzej/alias-releases/releases): either way the addon lands in `addons/alias_support` |

How to use them: [Clients](https://getalias.support/guide/integration/clients).

## Tools

Archives for Linux, macOS and Windows on each [release](https://github.com/emdzej/alias-releases/releases),
with `checksums.txt`:

- **aliasctl**: ALIAS from a terminal, for support people and whoever runs a workspace ([CLI](https://getalias.support/guide/integration/cli)).
- **alias-agent**: remote assistance and reports from a device with no app of its own.
- **alias-reporter**: a report window installed beside your product, for when it can't report itself.

## The API

- `spec/openapi.yaml`: the user API, which every client follows ([reference](https://getalias.support/guide/integration/api)).
- `spec/redact-vectors.json`: the redaction test cases, for checking a client of your own.

Versions match the service's: a release `X.Y.Z` here goes with ALIAS `X.Y.Z`, and works with later ones
in the same major version.
