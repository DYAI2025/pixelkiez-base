# Julia Provider Snapshot Reconciliation — PXK-88

Jira: PXK-88 (reconciliation), PXK-4 (baseline authority); parent PXK-79 / PXK-78  
Reconciled: 2026-09-30, completed 2026-10-01  
Donor repository: `DYAI2025/pixelkiez-base`, branch `pxk-4-julia-baseline-freeze`, base `master @ ca33fa5a4ab8170f62f6ea236689cbfc5b4a0853`  
Pre-reconciliation PR head: `ee028de6625333a8b6b679f5ac27e7688940bc84`  
Target repository: `DYAI2025/Julia-agent-harness`, `main @ db6dc536880ad00aa30f7abca66a70ea40a4a724` (contains only `README.md`; unchanged by PXK-88)

## 1. Why this reconciliation exists

PR #1 was opened on 2026-08-31 with every provider-core field marked `SOURCE_NEEDED`, because no ElevenLabs management capability was available then. On 2026-09-01 the agent was read read-only and documented on Confluence PXKEV 09; PXKEV 08 was updated to say the provider-core blocker was resolved. Git and Confluence therefore contradicted each other on provider-core status. PXK-88 removes that contradiction without closing any gap the provider read did not close.

## 2. Source map

| Role | Source | Binding |
|---|---|---|
| Baseline evidence and donor | `DYAI2025/pixelkiez-base / agents/julia/baseline/2026-08-31` | PR #1, branch `pxk-4-julia-baseline-freeze` |
| Field-level provider snapshot | Confluence PXKEV 09 `09 – Julia aktuelle ElevenLabs Provider-Konfiguration` | page `41713665`, version 2 (2026-09-30; v2 adds only an anti-drift banner, the provider values date from 2026-09-01) |
| PXK-4 gate and remaining gaps | Confluence PXKEV 08 `08 – PXK-4 Julia Baseline Freeze – Evidence & Blocker` | page `40861697`, version 2 (2026-09-01) |
| Provider read | ElevenLabs `get_agent_config`, agent `agent_9501m0xnatwqfne90mcst6kb1wj8`, read-only | 2026-09-01; no raw export stored in Git |
| Supplied prompt | `Eingefügter Text.txt`, file reference `file_000000005da482118c83147f45f1c69f` | normalized in `prompt-baseline.md` |
| Current Julia target architecture | Confluence page `75464705` (`11 – Julia GPT-Live Account-Agnostic Deployment Harness & Self-Installing Repository`) | referenced by the PXKEV 09 v2 anti-drift banner; not an input to this baseline |
| Future implementation target | `DYAI2025/Julia-agent-harness` | `main @ db6dc536880ad00aa30f7abca66a70ea40a4a724` |

Direction: the donor baseline is read by later slices; nothing flows back into it. PXK-88 adds no harness code to the target repository.

## 3. Promotion matrix

Each row compares the pre-reconciliation state (head `ee028de`) with the reconciled state. Only fields that PXKEV 09 v2 records as read were promoted.

| Field | Before | After | Evidence |
|---|---|---|---|
| Agent ID | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` | PXKEV 09 §1 |
| Agent branch/version | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` | PXKEV 09 §1 |
| Agent display name | `USER_STATED` | `VERIFIED_SNAPSHOT` | PXKEV 09 §1 |
| First Message | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT / DEFECT_PRESERVED` | PXKEV 09 §2 |
| LLM and generation parameters | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` | PXKEV 09 §3 |
| Provider system prompt | not recorded | `PARTIALLY_SUPPORTED` | PXKEV 09 §3; see §5 below |
| Voice ID, TTS model, voice parameters | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` (style, voice filter still `SOURCE_NEEDED`) | PXKEV 09 §4, §6 |
| ASR | not recorded | `VERIFIED_SNAPSHOT` | PXKEV 09 §5 |
| Turn eagerness, turn/silence/soft timeout | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` | PXKEV 09 §5 |
| Interruption thresholds | `SOURCE_NEEDED` | `SOURCE_NEEDED` | not in the read |
| Max conversation duration | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` (`600s`) | PXKEV 09 §6 |
| Background audio / noise | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` (no audible source evidenced) | PXKEV 09 §6 |
| Dynamic Variables | `PARTIAL_VERIFIED_PROJECT_CONTRACT`; binding `SOURCE_NEEDED` | 15 placeholders `VERIFIED_SNAPSHOT`; runtime population `SOURCE_NEEDED` | PXKEV 09 §7 |
| Knowledge Base / RAG | `SOURCE_NEEDED` | 8 bindings and RAG core `VERIFIED_SNAPSHOT`; IDs/digests `SOURCE_NEEDED` | PXKEV 09 §8 |
| Standalone/webhook tools | `SOURCE_NEEDED` | `VERIFIED_EMPTY_SNAPSHOT` | PXKEV 09 §9 |
| Built-in/system tools | `SOURCE_NEEDED` | `VERIFIED_NULL_SNAPSHOT` | PXKEV 09 §9 |
| MCP tools | `SOURCE_NEEDED` | `VERIFIED_EMPTY_SNAPSHOT` | PXKEV 09 §9 |
| Workflow | `SOURCE_NEEDED` | `VERIFIED_SNAPSHOT` (none found) | PXKEV 09 §9 |
| Procedures | `SOURCE_NEEDED` | `SOURCE_NEEDED` | PXKEV 09 §9: no reliable list |
| Guardrails | not recorded | enabled set `VERIFIED_SNAPSHOT`; detail `SOURCE_NEEDED` | PXKEV 09 §11 |
| Success Evaluations | `SOURCE_NEEDED` | `VERIFIED_EMPTY_SNAPSHOT` | PXKEV 09 §11 |
| Data Collection | not recorded | `VERIFIED_EMPTY_SNAPSHOT` | PXKEV 09 §11 |
| Provider tests | `SOURCE_NEEDED` | `SOURCE_NEEDED` | PXKEV 09 §11: `UNVERIFIED_EMPTY` |
| Security/override settings | `SOURCE_NEEDED` | `SOURCE_NEEDED` | PXKEV 09 §12 |
| Telephony/phone binding | `SOURCE_NEEDED` | `SOURCE_NEEDED` | PXKEV 09 §12 |
| `provider_exact_reproduction` | `false` / `BLOCKED_SOURCE_NEEDED` | `false` / `PARTIAL_SOURCE_NEEDED` | PXKEV 08 §9 |

## 4. Remaining gaps — kept open on purpose

These are the PXKEV 08 §8 gaps plus the partial surfaces this reconciliation found. None is closed by PXK-88, and none may be read as `false` or disabled:

1. traffic allocation;
2. telephony / phone / Twilio / SIP binding;
3. inbound/outbound channel binding;
4. agent authentication / signed URLs;
5. allowlists;
6. allowed runtime overrides;
7. privacy / retention;
8. recording;
9. call limits;
10. guardrail detail mode / thresholds;
11. voice filter;
12. Procedure list (dedicated Procedure read);
13. Julia-specific provider tests (dedicated agent-test read);
14. Dynamic Variable runtime population path;
15. Knowledge Base resource IDs and content digests;
16. interruption thresholds;
17. an immutable raw export of System Prompt and First Message.

The same list is machine-readable as `remaining_source_needed` in `baseline-manifest.json`.

## 5. Provider prompt versus repository prompt

PXKEV 09 records the provider-stored system prompt as read in full, with a length of about 22,658 characters. The repository prompt body in `prompt-baseline.md` (everything after the header separator) measures 23,046 characters, 388 more. `prompt-baseline.md` states it is a normalized snapshot, not a byte-for-byte provider export. Equality is therefore not established, and the provider prompt stays `PARTIALLY_SUPPORTED`. Closing this needs gap 17.

## 6. Digests

SHA-256 of the files at the PXK-88 reconciliation commit:

| File | SHA-256 |
|---|---|
| `prompt-baseline.md` | `f58893de5d343e342b4cc32e6c38023f1f6c38fff77fe3d970c8a514ebd8e1c5` |
| `golden-conversation-set.md` | `502c2df3deb6a99dabb36eb7cc6ad0294e9ccc2955680495162807e57f732503` |
| `regression-fixtures.md` | `200f45f0a64ef4c88d9163a893f52a3e84d280cb325bbe22507c59c7dd02da8b` |
| `provider-settings-inventory.md` (Git-side provider snapshot) | `619dbd85f2c056aa7152acf4d952a0d117b11925956736aeb5236df45661959e` |
| `baseline-manifest.json` | `ea380573bc14b1c7d2c2aea7e60d8f02bf85806ffb90e248f592f1a86d01516c` |

Aggregate baseline digest: `6476da7548d7f30816340574e11c797143ab3b61b501ffee1cffc84dc9c5fae8`

Reproduce from this directory:

```sh
shasum -a 256 baseline-manifest.json golden-conversation-set.md prompt-baseline.md provider-settings-inventory.md regression-fixtures.md | shasum -a 256
```

Digest scope:

- `prompt-baseline.md`, `golden-conversation-set.md` and `regression-fixtures.md` are byte-identical to their state before PXK-88.
- `baseline-manifest.json` carries the digests of the four Markdown artifacts above it; this file carries the manifest digest. `README.md` and this file are not digested, which avoids a circular dependency.
- No provider-side digest exists: the provider read is bound by agent ID, branch ID, version ID and the PXKEV 09 page ID and version, not by a hash of a raw export.

## 7. Authorities after the baseline

- PXK-6 owns the repair requirements for the defects frozen here.
- PXK-7 owns acceptance and release-gate semantics, including the regression run against this baseline.
- PXK-93 is the later provider-neutral implementation slice; it takes PXK-6 as its requirements authority and PXK-7 as its acceptance authority.
- PXK-4 and PXK-88 are handled as one baseline-reconcile work item.

## 8. Open PO decision — repository visibility

On 2026-10-01 both `DYAI2025/pixelkiez-base` and `DYAI2025/Julia-agent-harness` report visibility `public`. This baseline contains the full Julia prompt, the provider agent, branch, version and voice IDs, and a First Message naming a third person. Whether either repository should stay public is a product-owner decision. PXK-88 does not change visibility.

## 9. Scope boundary

PXK-88 made no guardrail repair, no provider mutation (ElevenLabs, OpenAI, Twilio), no change to the target repository and no change to the prompt, Golden Conversation Set or regression fixtures. It proves no behavior, provider deployment, live calling, legal eligibility or production readiness.
