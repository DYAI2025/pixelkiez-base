# Julia Baseline Freeze - 2026-08-31

Jira baseline authority: PXK-4  
Jira reconciliation: PXK-88  
Parent authorities: PXK-3 / PXK-78 / PXK-79  
Donor repository: `DYAI2025/pixelkiez-base`  
Branch: `pxk-4-julia-baseline-freeze`  
Base: `master @ ca33fa5a4ab8170f62f6ea236689cbfc5b4a0853`  
Pre-reconciliation PR head: `ee028de6625333a8b6b679f5ac27e7688940bc84`  
Target repository binding: `DYAI2025/Julia-agent-harness`, `main @ db6dc536880ad00aa30f7abca66a70ea40a4a724`  
Freeze date: 2026-08-31 Europe/Berlin  
Provider snapshot date: 2026-09-01  
Reconciled: 2026-09-30

## Purpose

This directory freezes the evidence-supported Julia behavior baseline before Guardrail Repair and binds the later read-only ElevenLabs provider-core snapshot without changing Julia behavior.

It is not a repaired prompt, a complete provider/workspace export, or proof of runtime behavior.

## Truth status

| Surface | Status | Evidence |
|---|---|---|
| Julia normalized system-prompt content | `USER_PROVIDED_INSPECTED` | `prompt-baseline.md`; source file reference `file_000000005da482118c83147f45f1c69f` |
| Provider system-prompt state | `PARTIALLY_SUPPORTED` | PXKEV 09 records a full read and approximate length; no immutable raw provider export is stored here |
| Prompt behavioral intent | `VERIFIED_FROM_SUPPLIED_PROMPT` | identity, mission, evidence rules, responsiveness, objection handling, hard-no policy |
| Preferred conversation behavior | `USER_STATED / PARTIAL_FIXTURE` | Architect source-map S021, user-provided first conversation behavior test, 2026-08-28 |
| Current problematic conversation | `USER_PROVIDED_REVIEWED` | PXKEV 02, page `40632321` |
| Agent identity and version | `VERIFIED_SNAPSHOT` | PXKEV 09 v2, page `41713665` |
| First Message | `VERIFIED_SNAPSHOT / DEFECT_PRESERVED` | PXKEV 09 v2; static `Herr Schnetzer` value is recorded, not repaired |
| LLM/provider core | `VERIFIED_SNAPSHOT` | PXKEV 09 v2 |
| Voice/TTS and ASR | `VERIFIED_SNAPSHOT` | PXKEV 09 v2 |
| Turn-taking core | `VERIFIED_SNAPSHOT` | PXKEV 09 v2 |
| Guardrails enabled | `VERIFIED_SNAPSHOT` | PXKEV 09 v2: `focus`, `prompt_injection` |
| Interruption/guardrail detail thresholds | `SOURCE_NEEDED` | not present in the provider read |
| Dynamic Variables | `PARTIALLY_SUPPORTED` | 15 placeholders verified; runtime population path not verified |
| Knowledge Base / RAG | `PARTIALLY_SUPPORTED` | eight bindings and RAG core verified; immutable resource IDs/digests not captured |
| Standalone/Webhook tools | `VERIFIED_EMPTY_SNAPSHOT` | `tool_ids=[]`, legacy tools `[]` |
| Built-in tools | `VERIFIED_NULL_SNAPSHOT` | read built-ins were `null` |
| MCP bindings | `VERIFIED_EMPTY_SNAPSHOT` | `mcp_server_ids=[]`, `native_mcp_server_ids=[]` |
| Active Procedures | `SOURCE_NEEDED` | dedicated Procedure read not available |
| Provider Success Evaluations | `VERIFIED_EMPTY_SNAPSHOT` | `[]` in the provider read |
| Provider Data Collection | `VERIFIED_EMPTY_SNAPSHOT` | `[]` in the provider read |
| Julia-specific provider tests | `SOURCE_NEEDED` | dedicated agent-test read required; global-list absence is not proof |
| Security/telephony/override/retention surface | `SOURCE_NEEDED` | not reliably exposed by the provider read: traffic allocation, telephony/channel binding, authentication, allowlists, overrides, retention, recording, call limits, voice filter |

## Frozen artifacts

- `prompt-baseline.md` - normalized snapshot of the supplied Julia prompt.
- `golden-conversation-set.md` - protected conversation qualities and positive fixture references.
- `regression-fixtures.md` - known pre-repair failure cases.
- `provider-settings-inventory.md` - field-level provider snapshot and evidence boundaries.
- `provider-snapshot-reconciliation.md` - PXK-88 source map, promotion matrix, digests, and remaining gaps.
- `baseline-manifest.json` - machine-readable baseline metadata and truth labels.

## Source and target map

`DYAI2025/pixelkiez-base / agents/julia/baseline/2026-08-31` is donor and baseline evidence.

`DYAI2025/Julia-agent-harness @ db6dc536880ad00aa30f7abca66a70ea40a4a724` is the future implementation target. PXK-88 does not add harness implementation there.

The full source map, the field-by-field promotion matrix, the remaining gaps and the SHA-256 digests are in `provider-snapshot-reconciliation.md`. Repository visibility of both repositories is an open PO decision recorded there; PXK-88 does not change it.

## Protected conversation DNA

The later Guardrail Repair must preserve, unless an explicit test shows a conflict with truth or safety:

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

## Known baseline defects - frozen, not repaired here

- static `Herr Schnetzer` provider First Message;
- fake human-biography framing around the Swabian/Stuttgart accent;
- automatic employee/owner-name disclosure risk;
- unsupported visibility, ranking, pricing, or action claims;
- no verified booking/CRM/mail tools despite action language;
- positive reinforcement of sexualized comments;
- unverified persistence of playful identity data;
- blank runtime-placeholder speech.

These remain repair requirements. PXK-6 owns the repair requirements, PXK-7 owns acceptance/release-gate semantics, and PXK-93 is the later provider-neutral implementation slice.

## Reproducibility boundary

The prompt/policy and reference artifacts are frozen. The provider-core state is snapshot-bound and materially more complete than the initial PR, but complete provider-exact reproduction remains false because channel, security, runtime-population, Procedure, test, and other workspace surfaces remain unresolved.

Missing visibility is never interpreted as `false` or disabled.

## No release implication

This baseline does not prove behavior, provider deployment, tool execution, live calling, legal eligibility, production readiness, or completion of the Julia harness.
