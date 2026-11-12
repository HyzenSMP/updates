# Commands

Every command on Hyzen SMP. Kept up to date as features ship; the date of the last change is in the git history.

## Homes

- `/sethome [name]` save a home
- `/home [name]` teleport to a home
- `/delhome <name>` delete a home
- `/homes` list your homes

## Teleport

- `/tpa <player>` ask to teleport to someone
- `/tpahere <player>` ask someone to come to you
- `/tpaccept` / `/tpdeny` answer a request (add a name if you have more than one)
- `/tptoggle` turn teleport requests on or off

## Random teleport

- `/rtp` (also `/wild`, `/randomtp`) pick Overworld, Nether or End. 3s warmup, cancelled if you move or get hit. Free.

## Money

- `/bal` your balance (also `/balance`, `/money`)
- `/pay <player> <amount>`
- `/baltop` richest players

## Hyzen Coins

A second currency, earned just by playing: 1 coin every 10 minutes AFK, 8 moving around, 6 mining or building, 5 fighting. AFK machines, minecarts, water streams and autoclickers earn at the AFK rate, and only one account per IP earns.

- `/hc` your coins, your current rate and time to the next coin
- `/hc top` most coins
- `/hcshop` spend coins: netherite ingot 75, netherite upgrade template 40, elytra 200 (1 a week), enchanted golden apple 100 (1 a day), Mending book 60, 2 shulker shells 25, 16 bottles o' enchanting 10

## Shop

- `/shop` opens the shop: End, Nether, Gear, Food and Materials pages. Left click buys, right click sells, shift for a stack
- `/sell` opens the sell window: drop items in, see the total, confirm
- `/sell hand` sell what you're holding
- `/sellall [item]` sell everything sellable, or all of one item
- `/worth [item]` what something sells for, `/worth list` for every price
- `/sellhistory` your past sales

## Auction house

- `/ah` open it (also `/auction`)
- `/ah <item>` search, e.g. `/ah diamond`. Also finds renamed items by their name
- `/ah seller <player>` (or `/ah @player`) everything one player is selling
- `/ah sell <price>` list what you're holding, or use the Sell button to pick anything from your inventory
- `/ah selling` your listings, click one to cancel it
- `/ah sold` your history (sold, bought, expired)
- `/ah expired` items that came back to you

Sellers get paid instantly. Right click a shulker to see inside before buying.

## Buy orders

- `/orders` open orders, best paying first. Click one to hand in the items from your inventory and get paid at once (also `/ah orders`)
- `/orders create <item|hand> <amount> <price each>` post what you want to buy. The money is held while the order is open. Use `hand` for potions, enchanted books and tipped arrows
- `/orders mine` your orders, click an open one to cancel it
- `/orders fill <id> [amount]`, `/orders cancel <id>`

Up to 5 open orders each. Delivered items go to your `/ah` mailbox. Orders end after 7 days and whatever was not filled is refunded.

## Chat

- `/msg <player> <message>` private message (also `/tell`, `/w`, `/pm`)
- `/r <message>` reply

Swearing is blocked in chat, messages, signs, item names and AH listings. Each blocked message is a warning; the third mutes you for a day, and warnings clear after 7 days.

## Settings

- `/settings` turn on or off: teleport requests, summon requests, public chat, payments, private messages, fast buy (skip the AH confirm), and where your scoreboard sits (right, top, above the hotbar, or hidden)

## Rewards

- `/daily` daily reward and login streak (miss a day and it starts over)
- `/leaderboard` (also `/lb`, `/top`) top money, kills, mob kills and playtime: today, this week, this month, all time. Money and kills update live

## Other

- `/rules`
- `/voicechat` (needs the Simple Voice Chat mod)

## Rank perks

```
Rank      Homes      AH listings   /rtp cooldown
Default   1          20            60s
Ember     3          25            25s
Blaze     5          30            20s
Inferno   10         40            15s
Phoenix   Unlimited  50            10s
```

Ranks also show as a name colour in chat and tab, with ranked players at the top of tab.

## Staff (not for players)

- Helper: `/kick`, `/warnings <player>`, `/co inspect`, `/co lookup` (block history), `/sc` staff chat, `/sus` players the anti-cheat flagged, `/perf` server performance
- Mod: everything above plus `/mute <player> <reason> <30m|12h|1d>`, `/unmute`, `/ban <player> <reason> <30m|12h|7d>`, `/unban`, `/banhistory`, `/vanish`, `/staffmode`, `/totempop`, `/tp`, `/bal <player>`. Mods are never combat tagged
- Admin: everything above plus `/ban ... blacklist` (permanent), `/banrollback <staff>`, `/gamemode`, `/co rollback`, `/co restore`, `/eco give|take|set`, `/hc give|take|set|check`, `/hz reload`
