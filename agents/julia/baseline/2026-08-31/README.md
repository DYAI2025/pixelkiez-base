# Julia Baseline Freeze — 2026-08-31

Jira: PXK-4  
Parent Epic: PXK-3  
Branch: `pxk-4-julia-baseline-freeze`  
Base repository state: `DYAI2025/pixelkiez-base@ca33fa5a4ab8170f62f6ea236689cbfc5b4a0853`  
Freeze timestamp: 2026-08-31 Europe/Berlin

## Purpose

This directory freezes the **evidence-supported Julia behavior baseline before Guardrail Repair**.

It is intentionally **not** a repaired prompt and **not** proof of the active ElevenLabs provider configuration.

## Truth status

| Surface | Status | Evidence |
|---|---|---|
| Julia system-prompt content | `USER_PROVIDED_INSPECTED` | File Library source `Eingefügter Text.txt`, created 2026-08-31 |
| Prompt behavioral intent | `VERIFIED_FROM_SUPPLIED_PROMPT` | identity, mission, evidence rules, responsiveness, objection handling, hard-no policy |
| Preferred conversation behavior | `USER_STATED / PARTIAL_FIXTURE` | Architect source-map S021, user-provided first conversation behavior test, 2026-08-28 |
| Current problematic conversation | `USER_PROVIDED_REVIEWED` | PXKEV Confluence page `02 – Transcript Review: Abweichungen und Agent-Guardrails` |
| ElevenLabs agent ID | `SOURCE_NEEDED` | no provider connection in current execution environment |
| ElevenLabs branch/version ID | `SOURCE_NEEDED` | no provider connection in current execution environment |
| ElevenLabs voice ID/model | `SOURCE_NEEDED` | no provider connection in current execution environment |
| Turn/interruption/latency settings | `SOURCE_NEEDED` | no provider connection in current execution environment |
| Active Procedures | `SOURCE_NEEDED` | no provider connection in current execution environment |
| Active Tools | `SOURCE_NEEDED` | no provider connection in current execution environment |
| First Message configured in provider UI | `SOURCE_NEEDED` | supplied prompt contains an opening example, but provider First Message surface is not verified |

## Frozen artifacts

- `prompt-baseline.md` — normalized snapshot of the supplied Julia prompt used as the baseline reference.
- `golden-conversation-set.md` — protected conversation qualities and known positive fixture references.
- `regression-fixtures.md` — known negative/current regression cases that must stay reproducible.
- `provider-settings-inventory.md` — explicit provider-only settings that remain unavailable rather than guessed.
- `baseline-manifest.json` — machine-readable baseline metadata and truth labels.

## Protected conversation DNA

The Guardrail Repair must preserve, unless an explicit test shows a conflict with truth/safety:

1. natural spoken German rather than script-reading;
2. short, phone-appropriate answers;
3. response contingent on the immediately preceding user turn;
4. clarification and simplification when the prospect does not understand;
5. professional drift recovery;
6. warm but non-manipulative delivery;
7. confidence without pressure;
8. one main question per turn;
9. permission for correction and disagreement;
10. hard-no respect.

## Known baseline defects — frozen, not repaired here

PXK-4 deliberately records these without changing them:

- fake human-biography framing around the Swabian/Stuttgart accent;
- `consultant_name` is directly exposed in runtime/handoff wording;
- some handoff examples name a consultant automatically;
- no verified provider booking/tool configuration is captured;
- the reviewed transcript contains unsupported visibility/pricing/action claims despite prompt-level guardrails;
- personal/sexual boundary handling was too positively reinforcing before redirection.

These belong to PXK-6, not PXK-4.

## Reproducibility boundary

This freeze is reproducible for **prompt-/policy-level evaluation** using the files in this directory.

It is **not yet reproducible for provider-level voice/conversation behavior** because the exact active ElevenLabs agent configuration cannot be read from the currently connected tools. Provider-level reproduction remains blocked until the exact agent configuration is exported or API-read and then added as immutable evidence.

## No release implication

This baseline freeze does not authorize live outbound calling, does not establish legal eligibility, and does not prove behavioral/platform validation.