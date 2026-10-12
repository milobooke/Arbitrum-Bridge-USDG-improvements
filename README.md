# Arbitrum Bridge USDG improvements

A clickable design prototype of the USDG incentives card for the [Arbitrum Bridge](https://portal.arbitrum.io/bridge). It is a static mock-up for internal review, not the live bridge. It uses a demo wallet and never sends anything.

**Live demo:** https://milobooke.github.io/Arbitrum-Bridge-USDG-improvements/

## What to try

1. With USDG selected and Arbitrum One as the destination, tick the Terms checkbox and press **Move funds**.
2. After the transfer is submitted, the USDG card slides in from the right (from the bottom on mobile).
3. Close it, then move funds again. The card comes back after every USDG transfer to Arbitrum One.
4. Pick ETH or ARB, or flip the direction to Arbitrum One → Ethereum, and move funds. The card does not appear.

## Card spec

| | |
|---|---|
| Trigger | The user presses Move funds with USDG as the asset and Arbitrum One as the destination chain |
| Timing | Shows after the transfer is submitted, never before, so it doesn't interrupt the transfer |
| Persistence | Stays open until the user closes it. Shows again after every USDG transfer to Arbitrum One |
| Placement | Desktop: fixed to the top right, slides in from the right edge, 360px wide. Mobile: full width above the bottom navigation |
| Tag | DRIP program |
| Headline | Earn incentivized rewards with your USDG |
| Body | Supply USDG to Morpho or GMX vaults and earn up to 8% APR. |
| Call to action | Learn More → https://arbitrumdrip.com/opportunities (opens in a new tab) |

The 8% APR figure was the top Drip rate on launch day (October 6, 2026). In production, pull it live or drop the number.

Rewards come from supplying USDG to third-party vaults, not from holding USDG, and the copy keeps to that.

## Files

- `index.html` is the whole prototype, with logos and icons inlined.
- `og.png` is the link preview image and `favicon.png` the browser tab icon.
