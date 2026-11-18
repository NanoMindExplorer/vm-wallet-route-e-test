# VM Wallet Route E Test

Minimal test dApp for WalletConnect Route E: it shows the pairing URI as plain text so a browser agent can read it without QR or clipboard.

- `index.html` + `bundle.js` — self-contained static page (esbuild bundle of `@walletconnect/sign-client` 2.25.0).
- The WalletConnect Project ID in the bundle is a public identifier.
- No secrets in this repo: no private keys, no keystores, no passwords. The page only creates a WalletConnect pairing and requests a `personal_sign` of a harmless test message on Sepolia (chain `eip155:11155111`).

Live: https://nanomindexplorer.github.io/vm-wallet-route-e-test/
