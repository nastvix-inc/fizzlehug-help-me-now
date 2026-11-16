# Fizzlehug Help Me Now: Parenting in Hard Moments

Tantrum, meltdown, hitting, refusing, or about to lose it yourself? Calm, shame-free steps and exact words to say, for kids aged 2 to 12.

Your child is screaming on the supermarket floor, refusing to get dressed, hitting their sibling, or frozen at the school gate. Or you are the one about to snap. Tell Claude what is happening, in your own words and your own language, and you get:

- **What's happening**, from your child's side, without blame
- **What to do right now**, in 2 to 4 short steps
- **What to say**, with exact words that fit your child's age
- **What to avoid**, the phrases that usually make it worse
- **Once it's calm**, how to reconnect and repair

When you are the one struggling (overwhelmed, angry, guilty after yelling, exhausted), you get grounding steps, words to say to yourself, and permission to pause.

This is the quick version of Help Me Now from [Fizzlehug](https://fizzlehug.com), a parenting-support app. It gets you through the next few minutes. For what comes after, each answer ends with a link to Fizzlehug's Help Me Now, which opens on a written guide for that exact situation and your child's age, with a practice to do together and a plan so it happens less often.

## Principles

- Never shames the parent or the child.
- No diagnoses or clinical labels, and no punishment advice.
- Short enough to read with one hand while the other is holding your child.
- Checks for safety first. If someone may be in danger, it points you to emergency services and crisis lines instead of giving parenting tips.

This plugin is not medical, psychological or emergency advice. If you are worried about your child's health or development, talk to your child's doctor.

## Try it

Once the plugin is installed, just describe the moment. For example:

1. "My 4-year-old is screaming on the floor of the supermarket because I said no to candy."
2. "My 7 year old cries at the school gate every morning and won't go in."
3. "I just yelled at my kids and I feel terrible."
4. "My 2-year-old keeps hitting me when I tell him it's time to leave the park."
5. "My daughter is 9 and came home saying nobody at school will play with her."

## What the plugin does and does not do

- It is a single skill: instructions and reference notes for Claude. It contains no code, runs no commands, and makes no network requests.
- It does not store or send anything. What you write stays in your conversation with Claude.
- A full answer ends with **one** link to Fizzlehug's Help Me Now (fizzlehug.com/help-me-now), never in a safety response. No account is needed to use it. The link can include your child's age and the kind of situation (for example `age=4&behavior=crying_meltdown&context=store`) so the page opens straight on the right guidance, plus `utm_source=claude` so Fizzlehug can see the visit came from this plugin. Nothing is sent unless you choose to open the link. Fizzlehug removes the child's age and situation from the address bar before any analytics can read it; see [Fizzlehug's privacy policy](https://fizzlehug.com/privacy).
- If you ask how to prevent it or for a plan for the coming days, Claude gives a short direction and points you to Fizzlehug, where the practices and plans live.
- If you say you do not want links, Claude will not mention Fizzlehug again in that conversation.

## Contents

```
.claude-plugin/plugin.json
skills/help-me-now/SKILL.md                    the method and response format
skills/help-me-now/references/safety.md        safety check and crisis resources
skills/help-me-now/references/fizzlehug-links.md  how the optional Fizzlehug link is built
```

## Feedback

Open an issue in this repository, or visit [fizzlehug.com](https://fizzlehug.com).

## License

MIT, see [LICENSE](LICENSE).
