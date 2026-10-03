# Niche Audit Engine

A full-stack web application that produces structured, institutional-grade brand audits through the Claude API.

## The problem

A thorough brand audit is high value and high effort, which makes it a bottleneck. Delivered manually it does not scale, and the parts that take longest are research and structure rather than judgment.

## The approach

Encode the audit methodology into the application so structure and research are handled systematically, and the human contribution is the interpretation that actually requires sixteen years of pattern recognition.

## Architecture

- **Frontend.** Next.js application, form-driven intake, structured report output
- **Backend.** Supabase for authentication, data and persistence
- **Reasoning.** Claude API, running a defined audit framework across multiple analysis dimensions
- **Delivery.** Structured report generation

## Stack

Next.js · Supabase · Claude API · Vercel

## Design decisions worth noting

**Methodology as product.** The value is not the model call, it is the framework the model is run inside. The same API with no methodology produces generic output.

**Structured output over prose.** Forcing structured responses makes results comparable across audits and usable downstream, rather than producing a wall of text per client.

**Multiple revenue models supported.** Built to run as subscription, pay-per-audit, or white-label, because the right model was not obvious at build time and the architecture should not decide it.

---

<!-- TO ADD: a screenshot of a sanitised report, the audit dimension list, and the data model.
     Never commit client audit data. -->
