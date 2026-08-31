# Julia Provider Settings Inventory — 2026-08-31

Purpose: record every provider-level behavior setting required for a complete baseline and explicitly distinguish inspected values from unavailable ones.

## Current execution capability

No connected ElevenLabs management connector/API was available during PXK-4 execution. Plugin discovery did not return an ElevenLabs management plugin. Therefore provider values below are **not guessed**.

## Inventory

| Surface | Required for complete freeze | Current value/evidence | Status |
|---|---:|---|---|
| ElevenLabs Agent ID | yes | unavailable | `SOURCE_NEEDED` |
| Agent display name | yes | user/project refers to `Julia` | `USER_STATED` |
| Agent branch/version ID | yes | unavailable | `SOURCE_NEEDED` |
| System Prompt | yes | supplied `Eingefügter Text.txt`; normalized repository snapshot pending/recorded in this baseline | `USER_PROVIDED_INSPECTED` |
| First Message UI field | yes | provider field not read; prompt includes an opening *example* only | `SOURCE_NEEDED` |
| Voice ID | yes | unavailable | `SOURCE_NEEDED` |
| Voice/model version | yes | unavailable | `SOURCE_NEEDED` |
| Language | yes | prompt defines German B2B first contacts | `VERIFIED_FROM_PROMPT`, provider setting `SOURCE_NEEDED` |
| Stability/similarity/style/speed | yes if configured | unavailable | `SOURCE_NEEDED` |
| Turn eagerness | yes | unavailable | `SOURCE_NEEDED` |
| Interruption sensitivity/thresholds | yes | prompt policy says do not interrupt, but provider value unavailable | `SOURCE_NEEDED` |
| Silence timeout / soft timeout | yes | unavailable | `SOURCE_NEEDED` |
| Max conversation duration | yes | unavailable | `SOURCE_NEEDED` |
| Background audio/noise settings | if configured | unavailable | `SOURCE_NEEDED` |
| LLM/model | yes | unavailable | `SOURCE_NEEDED` |
| Temperature / generation controls | if exposed/configured | unavailable | `SOURCE_NEEDED` |
| Dynamic Variables schema | yes | prompt visibly references company/prospect/compliance/handoff/audit variables; current shared contract is project v1.3 = 96 total / 95 custom DVs | `PARTIAL_VERIFIED_PROJECT_CONTRACT`; active provider binding `SOURCE_NEEDED` |
| Knowledge Base documents | yes if active | unavailable | `SOURCE_NEEDED` |
| RAG/full-context mode | yes if KB active | unavailable | `SOURCE_NEEDED` |
| System tools | yes if active | unavailable | `SOURCE_NEEDED` |
| Webhook tools | yes if active | unavailable | `SOURCE_NEEDED` |
| MCP tools | yes if active | unavailable | `SOURCE_NEEDED` |
| Procedures / Workflows | yes if active | unavailable | `SOURCE_NEEDED` |
| Success Evaluation criteria | yes for behavioral baseline | no executed/provider snapshot available | `SOURCE_NEEDED` |
| Tests tab cases/results | yes for provider behavior baseline | no executed/provider snapshot available | `SOURCE_NEEDED` |
| Security/override settings | yes | unavailable | `SOURCE_NEEDED` |
| Telephony/phone-number binding | deployment-specific | unavailable | `SOURCE_NEEDED` |

## Prompt-level settings that are known

The supplied prompt explicitly requires:

- German B2B first contact;
- warm, friendly, calm, authentic, attentive, adult, confident, factual, respectful, unobtrusive voice effect;
- explicit AI identity;
- truth > respect/autonomy > relevance > clarity > trust > appointment;
- one main question per turn;
- contingent responses rather than a visible questionnaire;
- do not interrupt;
- short marked-silence explanation during tool waits;
- audit-only evidence grounding;
- hard-no immediate stop;
- no fake booking or email sending.

These are **prompt policy**, not proof that ElevenLabs provider-level conversation-flow settings match the policy.

## Completion gate for provider-exact baseline

To upgrade this file from `PARTIAL` to `COMPLETE`, capture an immutable provider export/API read including at minimum:

1. Agent ID and active version/branch;
2. full System Prompt and First Message as stored by ElevenLabs;
3. Voice ID/model and all non-default voice parameters;
4. LLM/model and exposed generation parameters;
5. turn-taking/interruption/silence/duration settings;
6. active Dynamic Variables;
7. Knowledge Base document IDs/digests and retrieval mode;
8. active system/webhook/MCP tools and schemas;
9. Procedures/Workflows;
10. Analysis/Success Evaluation configuration;
11. Tests definitions and, separately, actual run results;
12. security/override configuration relevant to behavior.

Until then, **provider-exact behavioral reproduction is blocked** even though the prompt/policy baseline is frozen.