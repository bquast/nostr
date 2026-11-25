# How Nostr works

An interactive 3D film that follows one Nostr note: key, event, hash, signature, relays, subscriptions, client checks, outbox model, replies.

The keys, ids and signatures are real (secp256k1 BIP-340 Schnorr, SHA-256, NIP-19). The relays are simulated.

## Files

- `index.html`: the page (HTML, CSS and JS in one file)
- `vendor.js`: local bundle of three.js 0.187, noble-curves 2.4, noble-hashes 2.4, scure-base 2.4
- `vendor-entry.js`: the list of exports in `vendor.js`
- `*.woff2`: Inter, Space Grotesk, JetBrains Mono

## Rebuild vendor.js

    npm i three@0.187.0 @noble/curves@2.4.0 @noble/hashes@2.4.0 @scure/base@2.4.0 esbuild
    npx esbuild vendor-entry.js --bundle --format=esm --minify --outfile=vendor.js

## Deploy

GitHub Pages: deploy from the `master` branch, root folder. No build step.

Keys: Space play, [ ] chapters, 1-4 what-if switches, D go deeper, C camera, Shift+N labels, M sound.
