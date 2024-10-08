A micro-cli to watch your macOS pasteboard and emit the raw contents to stdout
as jsonl.

```bash
$ /opt/homebrew/bin/x-macos-pasteboard
{"types":{"public.utf8-plain-text":"L29wdC9ob21lYnJldy9iaW4veC1tYWNvcy1wYXN0ZWJvYXJk"},"change":9445,"source":"com.mitchellh.ghostty"}
{"change":9446,"types":{"public.utf8-plain-text":"JCAvb3B0L2hvbWVicmV3L2Jpbi94LW1hY29zLXBhc3RlYm9hcmQKeyJ0eXBlcyI6eyJwdWJsaWMudXRmOC1wbGFpbi10ZXh0IjoiTDI5d2RDOW9iMjFsWW5KbGR5OWlhVzR2ZUMxdFlXTnZjeTF3WVhOMFpXSnZZWEprIn0sImNoYW5nZSI6OTQ0NSwic291cmNlIjoiY29tLm1pdGNoZWxsaC5naG9zdHR5In0="},"source":"com.mitchellh.ghostty"}
```

Intended to be combined with [`xs`](https://github.com/cablehead/xs) as a generator.

## Install

```bash
brew install cablehead/tap/x-macos-pasteboard
```

## Release

```
swiftc main.swift -O -o x-macos-pasteboard

gh release create v0.8 ./x-macos-pasteboard \
  --title "v0.8 - First Binary Release" \
  --notes "This release contains the first precompiled macOS binary of x-macos-pasteboard."
```
