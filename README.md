# Shop
> **Tip:** All Fortnite cosmetics can be found at [Fortnite.GG/cosmetics](https://fortnite.gg/cosmetics)
## Requirements for Cosmetics

- **Version:** Must be from Chapter 2 Season 4 (Version 14.40) or earlier.
- **Pricing:** I dont care about the price, just make it reasonable (or free)
- **Cosmetic ID:** Must follow the correct format (see below).

**Item Shop Format:**
```json
{
    "//": "BR Item Shop Config",
    "daily1": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "daily2": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "daily3": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "daily4": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "daily5": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "daily6": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "featured1": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "featured2": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "featured3": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE},
    "featured4": {"itemGrants": ["ItemType:CosmeticID"], "price": PRICEHERE}
}
```
- **Daily Items:** `daily1` to `daily6`
- **Featured Items:** `featured1` to `featured4`
- **ItemType:** 'replace ItemType with the type of cosmetic, example: "AthenaCharacter:"'
- **Price:** 'change "PRICEHERE" to your preferred price, it could be free (make it 0) or 500'
- **CosmeticID:** 'change "CosmeticID" to your preferred ID (must match the ItemType), example: "CID_083_Athena_Commando_F_Tactical"'
  
## Cosmetic ID Formatting

Each cosmetic has a unique ID. Format them as:

```
ItemType:CosmeticID
```

**Examples:**

- **Skin:** `"AthenaCharacter:CID_083_Athena_Commando_F_Tactical"`
- **Emote:** `"AthenaDance:EID_Flare"`
- **Pickaxe:** `"AthenaPickaxe:Reaper"`
- **Backbling:** `"AthenaBackpack:BID_004_BlackKnight"`
- **Glider:** `"AthenaGlider:Glider_StarSurfer"`
- **Wrap:** `"AthenaItemWrap:GalaxyWrap"`
- **Loading Screen:** `"AthenaLoadingScreen:LoadingScreen_Galactic"`
- **Skydiving Contrail:** `"AthenaSkyDiveContrail:Contrail_Rainbow"`

> **Important:** Always wrap Cosmetic IDs in double quotes.

## Common Mistakes to Avoid

- **No Quotes:** Always put cosmetic IDs in double quotes.
- **Comma Errors:** Write numbers without commas (e.g., use `1200` not `1,200`).
- **Wrong Versions:** Do not use cosmetics from after Chapter 2 Season 4.

## Tips

- **Use VS Code:** It highlights JSON errors and keeps formatting clean.
- **Validate with AI Tools:** Tools like ChatGPT can help check your JSON before testing.
