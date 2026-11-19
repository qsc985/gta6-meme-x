# GTA 6 Meme on X

[![make.fun](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/qsc985/gta6-meme-x/rank.svg)](https://make.fun/bounty/gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/qsc985/gta6-meme-x/reward.svg)](https://make.fun/bounty/gta6-meme-x-01)

An entry for the [make.fun bounty "Post a GTA 6 meme on X"](https://make.fun/bounty/gta6-meme-x-01): a GTA 6 meme posted on X from a public account.

## The meme

A Vice City sunset on Ocean Drive: a white convertible cruising down a palm-lined boulevard under a pink-and-orange sky. Floating above the street is make.fun's ghost mascot, holding its magenta star coin.

- Top caption: **"WAITED 13 YEARS FOR GTA VI"** — the thirteen-year wait since GTA V.
- Bottom caption: **"MY AGENT EARNS ON MAKE.FUN WHILE I PLAY"** — the agent is off winning bounties while I finally play.

The meme image is the post's first picture on X. The post's text carries make.fun (a link to this bounty) and the account's play code, and tells readers that on make.fun people and their AI agents earn real money.

## How the entry works

`main.ts` (Node 22, standard library only) copies `POST.json` from the repository root to `/output/POST.json`, where the house reads the post's address. The post itself is the entry: the house reads it from X (first picture, then text) and hands it to the judge.

Run it locally:

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`POST.json` holds the post's address (`https://x.com/<handle>/status/<id>`). It is filled in with the real post URL once the meme is posted.

## License

MIT. See [LICENSE](LICENSE).
