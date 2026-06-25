# Get Rob Snyder to Review Your Sales Calls (Sort Of)

A skill that lets you paste a sales call transcript and get [*Rob Snyder's*](https://www.linkedin.com/in/rsnyder1) brutally honest feedback on it.

If you're not sure whether the call went well, or it seemed to go well but they ghosted, or you feel like you could have done a better job but aren't sure what's most important, give it a try.

Unlike just having a generic AI review - which gets you feedback that sounds right, but almost never works because *something else turned out to be more important* - this skill encodes **Rob Snyder's PULL Framework**, which is a causal model of purchases that's caused 50+ startups to go $0-$1M+ ARR, including $0-$25M ARR in 2 years and $0-$6M ARR in 8 weeks.

The results will probably surprise you. Often you'll get feedback that you've been trying to sell to people who would be weird to buy (even if they have relevant pain points and like your product). Or that the way you are pitching your product is convincing them not to buy.

For more on Rob Snyder's PULL framework: buy his book [*The Power of PULL*](https://www.amazon.com/Power-Pull-Customer-Successful-Founders/dp/1541705955),
read his newsletter [The Physics of Startups](https://thephysicsofstartups.substack.com/p/sales-problems-vs-product-market?utm_source=publication-search),
or, if you want the real Rob to help you quickly figure out the best way to position and sell your product for fast growth, [work with Rob](https://robsnyder.org/work-with-me).

## What this skill does

Give it a transcript of a sales call. It gives you an analysis in four layers:

1. **Did the buyer pull?** Was it real pull, or did you misinterpret it?
2. **What did the potential customer want to buy, if anything?** Was demand visible on the call, and if so, what exactly was it for?
3. **How did you perform?** How was your discovery and how did you position your product, and generally was your head in the right place?
4. **What to change?** What to do with this deal and generally?

## Example

[*HERE*](https://fathom.video/share/vd5WEudX4BMYDa_vtVzJMniKJsHoKMgB) is a real sales call, from a startup called [*Sliq*](https://www.getsliq.com). 

You can see my actual live review of the call [*HERE*](https://www.youtube.com/watch?v=3TsrrMSXIfg&t=9s).

Run this skill on the call's transcript, and you'll get an output like this (shortened):

> **PULL action: NO.** Every forward step was seller-prompted and seller-closed. The buyer's strongest move was deferring: *"we may not know yet till after maybe onboarding and even some time in the tool."*
>
> **Some PULL was visible, but no U (urgency/unavoidability).** The Project and Limitations are named: *"the biggest thing slowing us down is just getting the right leads... it takes a lot of time."* But there's no forcing function. They started outbound a month ago, they're still warming up inboxes, and the buyer argues against their own urgency: *"It's hard to automate it too much at this point because we don't know what's working or not yet."* Nothing breaks if this stays manual another quarter.
>
> **The seller positioned and demo'ed their product incorrectly.** The seller didn't position their product in a coherent way before demo'ing, so the buyer didn't understand it before looking at the tool. Then the seller just demoed their own outreach process, which had very little to do with what the buyer wanted to see. For this customer, the seller needed to position the product as *"an AI agent that automates your manual process of finding your best-fit leads."* Then would show an example of a complex lead search that the agent performed.
>
> **What to do:** This kind of customer is probably not the seller's best-fit customer, the one who will rip it out of your hands. These people might buy and succeed, but they might not, and that's not how you grow fast. Instead find people who can't not buy right now - for example, those who are already doing outreach and it's working but it's too manual and cannot be automated using existing outbound tools. Adjusting your positioning and demo will also help.


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

## License

See [LICENSE](LICENSE).
