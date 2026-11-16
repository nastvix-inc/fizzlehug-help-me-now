# Building the Fizzlehug link

Fizzlehug's Help Me Now at https://fizzlehug.com/help-me-now works without an account. A link can carry what the parent already told you, so the page opens straight on the written guidance for that exact moment, with a practice for next time, instead of asking the same questions again.

## Format

```
https://fizzlehug.com/help-me-now?age=<age>&behavior=<behavior>&trigger=<trigger>&context=<context>&utm_source=claude&utm_medium=plugin&utm_campaign=help-me-now
```

Always keep the three `utm_` parameters. Every other parameter is optional. The page ignores a value it does not recognise, so a wrong value never breaks the link; it only asks that question again. Leave out anything you are not sure of rather than guessing.

The order matters: `trigger` is only used when `behavior` is set, and `context` only when `trigger` is set. Give each parameter once.

## `age`

A whole number from 2 to 12. Leave it out if you do not know the age or the child is outside that range.

## `behavior` and `trigger`

Pick what the child is doing, then one of the triggers listed for it. Use `unknown` for "something else".

| `behavior` | The child is | `trigger` values |
| - | - | - |
| `crying_meltdown` | Crying or melting down | `denied_request` (did not get what they wanted), `had_to_leave` (had to stop or leave something: the playground, a visit, a game with friends), `had_to_stop` (a screen or game had to end), `tired` (tired or hungry), `overwhelmed` (too much noise or too many people), `unknown` |
| `refusing` | Refusing | `had_to_stop` (had to stop something or go somewhere), `limit` (a limit or "no"), `bedtime`, `getting_ready` (getting dressed or ready to go), `hygiene` (teeth, bath, washing), `going_to_school` (going to daycare or school), `routine_task` (another everyday task), `unknown` |
| `upset_cant_calm` | Upset and cannot calm down | `overwhelmed`, `tired` (worn out after a long day), `scared`, `unexpected_change`, `mistake_or_failure` (made a mistake or something went wrong), `unknown` |
| `aggressive` | Hitting, pushing, throwing | `denied_request`, `overwhelmed` (overwhelmed or frustrated), `limit`, `unknown` |
| `shutdown` | Shut down or frozen | `overwhelmed`, `scared`, `unexpected_change`, `unknown` |
| `scared_anxious` | Scared or anxious | `scared` (something specific scared them), `unexpected_change`, `sensory_overload` (too much noise or stimulation), `unknown` |
| `unknown` | Not sure | `tired`, `hungry`, `overwhelmed`, `unknown` |

## Another child or a sibling was involved (any age)

Set `trigger=social_conflict`, add `peer`, and set `behavior` to how the child is reacting. Without `behavior` the page keeps only the age.

| `peer` | What happened | Ages |
| - | - | - |
| `aggression_received` | Someone hurt their child (hit, pushed, bit, said mean things) | all |
| `hurt_other` | Their child hurt someone | all |
| `conflict_one_kid` | A fight over a toy or a game; from 6, also a falling out or "not fair" | all |
| `excluded` | Left out | 3 and up |
| `sibling` | A brother or sister | all |
| `repeated` | It keeps happening with the same child | 5 and up |

How the child is reacting (`behavior`):

- Ages 2 to 5: `crying_meltdown`, `aggressive` (angry, hitting or grabbing), `shutdown` (quiet or frozen), `scared_anxious` (scared or clingy).
- Ages 6 to 12: the same four, plus `refusing` (refusing to talk about it) and `upset_cant_calm` (hurt or sad about it).

## `context`

`home`, `playground`, `store`, `public_place`, `on_the_way`, `visiting`, `daycare` (ages 5 and under), `school` (6 and up), `after_school` (6 and up), `unknown`.

## Parent branch

The parent branch cannot be pre-filled. Link to the page with the tracking parameters only:

```
https://fizzlehug.com/help-me-now?utm_source=claude&utm_medium=plugin&utm_campaign=help-me-now
```

## Examples

- 4-year-old, meltdown in a store after a "no":
  `https://fizzlehug.com/help-me-now?age=4&behavior=crying_meltdown&trigger=denied_request&context=store&utm_source=claude&utm_medium=plugin&utm_campaign=help-me-now`
- 3-year-old will not go to bed:
  `https://fizzlehug.com/help-me-now?age=3&behavior=refusing&trigger=bedtime&context=home&utm_source=claude&utm_medium=plugin&utm_campaign=help-me-now`
- 5-year-old screaming because it is time to leave the playground:
  `https://fizzlehug.com/help-me-now?age=5&behavior=crying_meltdown&trigger=had_to_leave&context=playground&utm_source=claude&utm_medium=plugin&utm_campaign=help-me-now`
- 8-year-old left out at the playground, crying:
  `https://fizzlehug.com/help-me-now?age=8&behavior=crying_meltdown&trigger=social_conflict&peer=excluded&context=playground&utm_source=claude&utm_medium=plugin&utm_campaign=help-me-now`
- 6-year-old hit their little brother:
  `https://fizzlehug.com/help-me-now?age=6&behavior=aggressive&trigger=social_conflict&peer=sibling&context=home&utm_source=claude&utm_medium=plugin&utm_campaign=help-me-now`

## Other Fizzlehug pages

Mention these only when the parent asks for more reading, tools or an app:

- Parent Guide (free articles): https://fizzlehug.com/parent-guide
- Articles for one age band: https://fizzlehug.com/parent-guide/ages/2-3 (also `4-5`, `6-8`, `9-12`)
- How Fizzlehug works: https://fizzlehug.com/how-it-works
