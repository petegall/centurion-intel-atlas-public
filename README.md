# Centurion Intel Atlas (Public)

This repository contains sanitized, read-only atlas outputs generated from the private Centurion system atlas.

Purpose:
- publish safe system summaries
- support tool access through stable public artifacts
- provide a clean public atlas surface for documentation and automation

Public endpoints:
- `/` — landing page
- `/atlas` — atlas index (JSON)
- `/system` — system map (Markdown)
- `/graph` — system graph (JSON)

Canonical public artifacts:
- `outputs/index.json`
- `outputs/SYSTEM.md`
- `outputs/SYSTEM.graph.json`

This repository should not contain:
- secrets
- raw private snapshots
- Airtable schema dumps
- Make blueprints
- unpublished internal system details

Architecture:
private atlas repo → generated safe outputs → public mirror repo → Vercel-hosted public endpoints

Source of truth for internal system inputs lives in the private repository: `centurion-intel-atlas`
