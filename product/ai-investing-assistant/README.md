# An always-on AI CIO for retail investors

> **Goal:** give everyday investors a 24/7 AI adviser that watches the market, knows their portfolio and alerts them first.
>
> **How:** a multi-agent system on top of a cross-asset rating engine, with memory and a proactive agent.
>
> **Result:** 480K users and US$1M peak ARR. My role: co-founder and CEO, product and AI architecture lead.

---

## What it does
- Answers questions about any stock, ETF or crypto asset, with the user's own portfolio in mind
- Watches the market and the user's holdings around the clock, and speaks up first when something matters
- Lets users set up recurring reports and price monitors just by asking in the chat

## How it's built

**1. Specialist agents, not one generalist.** 17 agents each own one job (financials, valuation, industry, technicals and so on), and requests are routed to the right ones. Stocks are classified by style, structure and theme, so each agent gets the metrics and industry framework that actually fit.

**2. A rating engine underneath.** Every analysis starts from a cross-asset rating engine: stocks, ETFs and crypto, each scored against their own industry by percentile, with a confidence flag where data is thin. 159 outside "skills" were consolidated into 28, and every one reads the ratings first.

**3. Memory and proactivity.** I led the team to ship cross-session memory (who the user is, what they hold, what they care about) and a proactive agent that reacts to market events and the user's behaviour.

**4. Two principles that kept it simple:**
- **Same data for everyone, different presentation.** The scores never change by user; only how much detail is shown. Matching the presentation to the type of user lifted simulated NPS on the same stock from 0 to 60.
- **Capabilities separate from screens.** Agents return structured data that the app turns into standard charts, so new capabilities don't need new UI work.

## Related
- [Stock 360 research method](../../research/stock-360/): the research instruction set behind the reports
- [Perceived value and NPS](../pv-nps/) and [testing with simulated users](../ai-user-simulation/): how we decided what to build

---

*Brand names, internal metrics and team details have been removed. The engineering stack was built by the team; I designed the product and the AI architecture.*
