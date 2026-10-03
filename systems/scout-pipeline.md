# Scout + Soul Pipeline

An autonomous pipeline that sources, enriches, qualifies and engages prospects without manual input.

## The problem

Business development for a consultancy is a volume problem disguised as a relationship problem. Finding and qualifying the right people consumes the hours that should go into the actual work, and it is the first thing dropped when client delivery gets busy.

## The approach

Separate the parts that genuinely need judgment from the parts that do not. Sourcing, enrichment and first-pass qualification are rules and data. Only the final conversation needs a human.

## Architecture

- **Sourcing.** Apify for collection, Apollo for contact and company data
- **Orchestration.** n8n workflows chaining collection, enrichment, scoring and routing
- **Storage.** Supabase as the system of record for prospects and pipeline state
- **Qualification and messaging.** Claude API for scoring against an ideal customer profile and drafting in-voice outreach

## Stack

n8n · Supabase · Apify · Apollo · Claude API

## Design decisions worth noting

**n8n over custom code.** Visual workflow orchestration made the pipeline inspectable and editable without a deploy cycle, which mattered more than elegance for something iterated weekly.

**Supabase as the spine.** A real database rather than spreadsheets meant pipeline state survived workflow changes and could be queried by other systems.

**Scoring before drafting.** Qualifying first and drafting second cuts API cost substantially and keeps output quality high, because the model only writes for prospects worth writing to.

---

<!-- TO ADD: a workflow diagram, the scoring criteria (sanitised), and the enrichment field list.
     Never commit API keys or prospect data. -->
