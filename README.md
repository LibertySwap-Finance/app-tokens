# app-tokens

Whitelisted token assets and token list for LibertySwap (PulseChain).

This repository maintains the official token list used by LibertySwap and LibertyX.

### Token JSON Schema
Every token must follow this structure:

```json
{
  "chainId": 369,
  "address": "0x...",
  "name": "Token Name",
  "symbol": "SYMBOL",
  "decimals": 18,
  "logoURI": "https://raw.githubusercontent.com/LibertySwap-Finance/app-tokens/main/token-logo/0x...png"
}
```

Required fields: chainId, name, address, decimals, symbol, logoURI.

## How to Add or Update a Token

1. Fork this repository.
2. Add your token at the end of the token array in **libertyx-tokenlist.json**.
3. Ensure the token strictly follows the schema above.
4. Place the token logo inside the **token-logo/** folder (use the token address as the filename, e.g. **0x15D38573d2feeb82e7ad5187aB8c1D52810B1f07.png**).
5. Commit your changes and open a **Pull Request** to the **dev** branch.

***Example Token Entry JSON***
```json
{
  "chainId": 369,
  "address": "0x15D38573d2feeb82e7ad5187aB8c1D52810B1f07",
  "name": "USD Coin from Ethereum",
  "symbol": "USDC",
  "decimals": 6,
  "logoURI": "https://raw.githubusercontent.com/LibertySwap-Finance/app-tokens/main/token-logo/0x15D38573d2feeb82e7ad5187aB8c1D52810B1f07.png"
}
```

# Important Notice:

* Not every token will be accepted.
* All submissions are subject to review and approval by the LibertyX team.
* You must provide a proper logo and accurate token details.

# Disclaimer
After submitting a Pull Request, please be patient. We review submissions as time allows and do not follow a strict first-come, first-served order.