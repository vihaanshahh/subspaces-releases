# subspaces.si

Public beta downloads for [subspaces.si](https://subspaces.si), a free, ad-funded AI coding IDE.

## Downloads

Release: [v0.1.0-beta](https://github.com/vihaanshahh/subspaces-releases/releases/tag/v0.1.0-beta)

| Platform | Archive |
| --- | --- |
| macOS Apple silicon | [subspaces-si-0.1.0-darwin-arm64.tar.gz](https://github.com/vihaanshahh/subspaces-releases/releases/latest/download/subspaces-si-0.1.0-darwin-arm64.tar.gz) |
| macOS Intel | [subspaces-si-0.1.0-darwin-x64.tar.gz](https://github.com/vihaanshahh/subspaces-releases/releases/latest/download/subspaces-si-0.1.0-darwin-x64.tar.gz) |
| Linux x64 | [subspaces-si-0.1.0-linux-x64.tar.gz](https://github.com/vihaanshahh/subspaces-releases/releases/latest/download/subspaces-si-0.1.0-linux-x64.tar.gz) |
| Checksums | [SHA256SUMS](https://github.com/vihaanshahh/subspaces-releases/releases/latest/download/SHA256SUMS) |

## Install

Requires Node.js 22.

Unpack the archive for your platform, change into the extracted folder, and start the app:

```sh
tar -xzf subspaces-si-0.1.0-linux-x64.tar.gz
cd subspaces-si-0.1.0-linux-x64
./start
```

Use the `darwin-arm64` or `darwin-x64` archive name on macOS. The extracted folder name matches the archive name without `.tar.gz`.

Optional: copy `.env.example` to `.env` and fill in model or ad keys.

If macOS Gatekeeper blocks the app:

```sh
xattr -dr com.apple.quarantine subspaces-si-0.1.0-darwin-arm64
```

Use the folder you extracted.

## Verify checksums

Download `SHA256SUMS` next to the archive, then check the file you downloaded.

Linux:

```sh
sha256sum -c SHA256SUMS
```

macOS:

```sh
shasum -a 256 -c SHA256SUMS
```

`sha256sum` and `shasum` report a failure for any archive you did not download. That is expected. Confirm the line for your archive says `OK`.
