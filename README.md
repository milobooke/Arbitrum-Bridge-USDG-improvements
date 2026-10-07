# Arbitrum Bridge USDG improvements

A clickable design prototype of the USDG incentives banner for the [Arbitrum Bridge](https://portal.arbitrum.io/bridge). It is a static mock-up for internal review, not the live bridge. Wallet actions are turned off.

**Live demo:** https://milobooke.github.io/Arbitrum-Bridge-USDG-improvements/

## What to try

- **Token selection:** the banner appears only when USDG is the selected token. Pick ETH or ARB in the token selector and it goes away.
- **Direction:** the swap arrows flip Ethereum → Arbitrum One and back. The banner shows in both directions.
- **Dismiss:** closing the banner keeps it hidden in that browser. "Show banner again" in the top strip resets it.
- **Mobile:** narrow the window, or open the link on a phone, to see the mobile layout.

## Banner spec

| | |
|---|---|
| Headline | Earn incentivized rewards with your USDG |
| Subline | Supply USDG to Morpho or GMX vaults — up to 8% APR. |
| Call to action | View vaults → https://arbitrumdrip.com/ (opens in a new tab) |
| When it shows | The selected token is USDG, as the source or destination asset |
| Placement | Top of the bridge column, above the transfer panel, same 600px width, 12px gap |
| Dismissal | Close button hides it; remember the choice per browser |
| Mobile | Sits between the Bridge / Txns / Buy tabs and the transfer panel. "View vaults" becomes a full-width button |

The 8% APR figure was the top Drip rate on launch day (October 6, 2026). In production, pull it live or drop the number.

Rewards come from supplying USDG to third-party vaults, not from holding USDG, and the copy keeps to that.

## Files

- `index.html` is the whole prototype, with logos and icons inlined.
