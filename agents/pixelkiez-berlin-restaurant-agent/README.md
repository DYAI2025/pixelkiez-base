# Pixelkiez Berlin Restaurant Voice Agent

Version: 2026-08-26

This package contains a compiled ElevenLabs-oriented appointment-agent build plus a Berlin restaurant industry capsule, a synthetic restaurant fixture, validated build inputs, restaurant-specific evaluation scenarios, and production-readiness guidance.

## Current status

- Architecture/package compile: PASS
- Input schema validation: PASS
- Selected simulation hooks: reservation path (F1), offer clarity (F2)
- AI disclosure: required and included
- Recording: OFF
- Calendar/CRM/transfer/voicemail: UNVERIFIED
- Live cold-call production status: BLOCKED_EXTERNAL / LEGAL_REVIEW_REQUIRED

## Why the sample prospect is synthetic

The compiler requires a prospect identity and a validated audit packet. No real Berlin restaurant was supplied, so this package deliberately uses a synthetic website fixture rather than inventing findings about a real business.

## How to use for a real restaurant

1. Supply the real restaurant identity and approved lead source.
2. Run a prospect-specific website audit and normalize it into the Website Audit Packet schema.
3. Externally determine the concrete campaign/lead compliance state. The agent itself may never self-authorize calling.
4. Compile a new prospect-specific agent package using the same Berlin restaurant industry capsule.
5. Configure ElevenLabs telephony, voice, conversation flow and tools.
6. Run simulation/adversarial evals.
7. Only after legal/compliance, tool, offer and deployment gates pass may the campaign be treated as live-call eligible.

## Design objective

Qualified human handoff after genuine relevance, not maximum raw meeting count.
