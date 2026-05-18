# PULL Call Analyzer

A [Claude Skill](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview)
that analyzes sales call transcripts using **Rob Snyder's PULL Framework**.

The PULL Framework states that buyers would be weird to buy UNLESS they have a
**P**roject on their to-do list that's **U**navoidable right now, and their
**L**ist of available options have **L**imitations.

For more on the framework: buy [*The Power of PULL*](https://www.amazon.com/Power-Pull-Customer-Successful-Founders/dp/1541705955),
read [The Physics of Startups](https://thephysicsofstartups.substack.com/p/sales-problems-vs-product-market?utm_source=publication-search),
or [work with Rob](https://robsnyder.org/work-with-me).

## What it does

Give it a transcript of a sales call, discovery call, demo, or pitch. It returns
a strict, evidence-bound diagnosis in four layers:

1. **Did PULL happen?** — did the buyer take a real PULL action.
2. **Was PULL visible?** — was a coherent Project / Unavoidability / Limitations
   structure present on the call.
3. **How did the seller perform?** — did they look for PULL, test it, fit the
   pitch to it.
4. **What to change?** — what to do with this deal and who the real buyer is.

Every claim is backed by a direct quote or by the conspicuous absence of one.

## Repo structure

```
pull-call-analyzer/
├── SKILL.md                      # how to apply PULL to a transcript
└── references/
    └── pull-framework.md         # canonical definition of PULL
```

## How to use it

### In Claude.ai or the Claude apps

Upload this skill under **Settings → Capabilities → Skills** (availability
depends on your plan). Once installed, paste or attach a call transcript and
ask for an analysis.

### With Claude Code or the Claude Developer Platform

Place the `pull-call-analyzer/` folder where your skills are loaded from, then
invoke it on any transcript. See the
[Agent Skills documentation](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview)
for the current setup steps.

## Output

Every run begins with a fixed header identifying the framework and pointing to
Rob's book, newsletter, and advising practice, followed by the four-layer
analysis.

## Note on `references/pull-framework.md`

The analyzer treats `references/pull-framework.md` as the source of truth for
*what PULL is*; `SKILL.md` only governs *how to apply it*. Edit the reference
file to update framework definitions; edit `SKILL.md` to change how analysis
is structured or formatted.

## License

See [LICENSE](LICENSE).
