# Ally Support

A UCP3 module for Stronghold Crusader and Stronghold Crusader Extreme. AI allies help each other
the way they already help the player: they answer each other's requests for goods (by their AIC
trade minimum), rich lords send gold, they come to each other's aid, and an AI that helps anyone
sends 75% of its attack army and keeps the rest home.

What the module does, in plain English, is in `module/locale/description-en.md`; how it does it
is in the comment at the top of `module/init.lua`.

## Notes on the settings

- **Recruiting gold on top of the AI character's own:** a lord's recruiting gold is its AI
  character's "recruit gold threshold" plus this value. The game makes an AI hold that
  threshold before it spends each month (often only 0-100); the default adds roughly the price
  of a handful of troops.
- **Call the helpers home sooner:** while the helpers are away their lord doesn't attack anyone,
  so a long stay also holds back its own attack. After a help ends, a lord waits 3 months, or
  until it has set out on its own attack, before it helps again.

## Working on it

1. Edit under `module/`.
2. `python tools/publish.py --bump` - raises the last version slot and copies the module to
   `ucp/modules/ally-support-<version>`. Do this with the game closed.
3. In the UCP GUI press F5, then apply.
4. Commit and tag: `git commit -am "<version> - <what changed>" && git tag v<version>`.

## Per-character AIC settings

Customizations supplies defaults. With AIC Loader 1.1.1 or later in the 1.x series, add
any of the following integer fields to the existing `Personality` object for a character.
Omit a field to use the corresponding Customizations value, or reset the AIC to restore
those values. The global feature switches still control which kinds of aid are enabled.

| AIC field | Values and whose setting applies |
| --- | --- |
| `AllySupportGoldKeep` | Donor reserve, 0–100,000 gold. Also used for player gold requests. AI-to-AI requests from weak allies can use up to half the reserve when that option is enabled. |
| `AllySupportRecruitGoldBuffer` | Recipient's extra recruiting reserve above its native threshold, 0–5,000 gold. |
| `AllySupportGoldSharePercent` | Donor's share of excess gold offered without a gold request, 0–100%. Zero turns off these gifts. |
| `AllySupportMonthlyGivePercent` | Donor's monthly goods and gold allowance with the relevant stock protection enabled, 0–100%. Zero disallows transfers subject to that limit. |
| `AllySupportArmySharePercent` | Helper's army share, 0–100%. Zero keeps the original game behaviour for army reserves. 100 keeps none of this army back. |
