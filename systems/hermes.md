# Hermes

An AI assistant running on Telegram, self-hosted on a DigitalOcean VPS, reachable from anywhere without opening a laptop.

## The problem

The useful version of an AI assistant is the one available in the ninety seconds between other things, from a phone, in a queue, in a taxi. Browser-based tools lose that window.

## The approach

A persistent assistant on the messaging app already open on the phone, hosted on infrastructure under my own control rather than a third-party wrapper, with access to the context it needs to be useful rather than generic.

## Architecture

- **Interface.** Telegram Bot API, conversational, mobile-first
- **Host.** DigitalOcean VPS, self-managed, always on
- **Reasoning.** Claude API
- **Integrations.** Email, plus connected data sources

## Stack

DigitalOcean · Telegram Bot API · Claude API · Node.js

## Design decisions worth noting

**Self-hosted on purpose.** Owning the deployment means owning the data path, the uptime and the cost model. It also means actually learning the deployment, which is the part that transfers to every future system.

**Messaging as interface.** No new app to adopt, no login, no friction. Adoption problems are usually interface problems.

---

<!-- TO ADD: setup and deploy instructions, environment variable list (names only, never values),
     and the integration list. Never commit tokens or keys. -->
