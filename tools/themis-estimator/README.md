# Themis Estimator

An interactive scoping and estimation tool. Branching discovery questions, scope-depth modelling, market tier comparison, and a generated proposal at the end.

**Open `index.html` in any browser. No build step, no dependencies, no server.**

## What it does

Four steps of discovery produce a scoped engagement with a named recommendation, a phased process, and an investment range, generated from the answers rather than selected from a menu.

## How it is built

A single self-contained HTML file. Vanilla JavaScript, no framework, no build pipeline. The pricing model lives in one clearly marked configuration object at the top of the script, so rates change in one place and everything downstream recalculates.

## Design decisions worth noting

**Scope moves, price logic does not.** The depth control adjusts how much work exists, never the rate. Letting a visitor drag a rate downward on your own site is self-sabotage.

**Floor pricing, not ranges.** The headline figure is where engagements start, with the upper bound in supporting text. You never publish a number you cannot defend upward.

**Tier comparison as positioning.** Rather than hiding the alternatives, the tool shows freelance, boutique, independent and agency side by side, so the recommendation is a reasoned position rather than an assertion.

**Rules-based, deliberately.** Pricing is deterministic rather than model-generated. An AI should never improvise a number a client is going to screenshot.
