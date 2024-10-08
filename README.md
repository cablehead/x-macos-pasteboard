## Release

```
swiftc main.swift -O -o x-macos-pasteboard

gh release create v0.8 ./x-macos-pasteboard \
  --title "v0.8 - First Binary Release" \
  --notes "This release contains the first precompiled macOS binary of x-macos-pasteboard."
```
