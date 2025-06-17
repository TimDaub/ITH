# Etherium (ITH)

This is the most direct fork possible of the canonical WETH (Wrapped Ether) contract deployed at [0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2](https://etherscan.io/address/0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2#code).

## Minimal Changes

The only modifications made from the original WETH contract are:
- Contract name: `WETH9` → `Etherium`
- Token name: `"Wrapped Ether"` → `"Etherium"`
- Token symbol: `"WETH"` → `"ITH"`
- Copyright: Added `2025 Etherium Fundation` to existing Dapphub copyright

## Verification

You can verify this is a direct fork by running a diff between this contract and the original WETH source code. Use any standard Unix diff tool or online diff checker to confirm that only the parameters mentioned above have been changed.

```bash
diff original-weth.sol src/Etherium.sol
```

The contract maintains 100% functional compatibility with WETH, including all the same functions, events, and behavior.

## Build

```shell
$ forge build
```

## Deploy

For CREATE2 deployment, use the compiled bytecode from `out/Etherium.sol/Etherium.json`.