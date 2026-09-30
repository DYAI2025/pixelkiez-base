# Julia Provider Settings Inventory — 2026-08-31 baseline, provider snapshot 2026-09-01

Purpose: record every provider-level behavior setting required for a complete baseline and explicitly distinguish verified snapshot values from unavailable ones.

Jira: PXK-4 (baseline authority), PXK-88 (reconciliation)  
Provider evidence: Confluence PXKEV 09 `09 – Julia aktuelle ElevenLabs Provider-Konfiguration`, page `41713665`, version 2 (read 2026-10-01)  
Provider read: ElevenLabs `get_agent_config` for `agent_9501m0xnatwqfne90mcst6kb1wj8`, read-only, 2026-09-01, evidence class `USER-PROVIDED ELEVENLABS PROVIDER READ / READ-ONLY`  
Summary authority: Confluence PXKEV 08, page `40861697`, version 2

Every `VERIFIED_SNAPSHOT` value below is copied from PXKEV 09 v2. No immutable raw provider export is stored in this repository; the values are snapshot-bound to the 2026-09-01 read, not to the live agent.

## Execution history

- 2026-08-31 (PXK-4): no ElevenLabs management connector/API was available; every provider field was recorded as `SOURCE_NEEDED` and not guessed.
- 2026-09-01: the agent was read read-only through the ElevenLabs hosted MCP / AI architect and documented on PXKEV 09.
- 2026-09-30 (PXK-88): this inventory was reconciled against PXKEV 08/09. Only fields the provider read actually covers were promoted; every surface the read does not expose stays `SOURCE_NEEDED`.

## 1. Agent identity and versioning

| Surface | Value | Status |
|---|---|---|
| Agent name | `Julia` | `VERIFIED_SNAPSHOT` |
| Agent ID | `agent_9501m0xnatwqfne90mcst6kb1wj8` | `VERIFIED_SNAPSHOT` |
| Versioning | enabled | `VERIFIED_SNAPSHOT` |
| Main branch | `agtbrch_7501m0xnavnjf9k9y583cgybgf9g` | `VERIFIED_SNAPSHOT` |
| Current branch | `agtbrch_7501m0xnavnjf9k9y583cgybgf9g` | `VERIFIED_SNAPSHOT` |
| Current version | `agtvrsn_4001m1cgzbrtfky9v6nmknyknpe2` | `VERIFIED_SNAPSHOT` |
| Branches | only `Main` | `VERIFIED_SNAPSHOT` |
| Traffic allocation | not reliably read | `SOURCE_NEEDED` |

## 2. First Message

| Surface | Value | Status |
|---|---|---|
| First Message (provider-stored) | „Schönen guten Tag Herr Schnetzer! Das freut mich, dass ich Sie erreiche. Mein Name ist Julia und ich bin eine KI Sprachagentin. Ich arbeite für die Agentur PixelKiez aus Berlin, sagt Ihnen unser Name was?“ | `VERIFIED_SNAPSHOT / DEFECT_PRESERVED` |

The static `Herr Schnetzer` salutation is a baseline defect (PXK-6), recorded here and not repaired.

## 3. LLM and prompt

| Surface | Value | Status |
|---|---|---|
| LLM | `gemini-3.7-flash` | `VERIFIED_SNAPSHOT` |
| Reasoning effort | `low` | `VERIFIED_SNAPSHOT` |
| Temperature | `0.66` | `VERIFIED_SNAPSHOT` |
| Max tokens | `-1` | `VERIFIED_SNAPSHOT` |
| Reasoning summary | `false` | `VERIFIED_SNAPSHOT` |
| Default personality | disabled (`ignore_default_personality=true`) | `VERIFIED_SNAPSHOT` |
| Timezone | `Europe/Berlin` | `VERIFIED_SNAPSHOT` |
| Cascade timeout | `4s` | `VERIFIED_SNAPSHOT` |
| Backup LLM 1 | `gemini-2.5-flash` | `VERIFIED_SNAPSHOT` |
| Backup LLM 2 | `qwen35-397b-a17b` | `VERIFIED_SNAPSHOT` |
| System prompt (provider-stored) | read in full on 2026-09-01; length about 22,658 characters | `PARTIALLY_SUPPORTED` |
| System prompt (repository) | `prompt-baseline.md`, normalized from the user-provided `Eingefügter Text.txt` | `USER_PROVIDED_INSPECTED` |
| Language | prompt defines German B2B first contacts; no separate provider language field in the read | `VERIFIED_FROM_PROMPT`, provider field `SOURCE_NEEDED` |

The repository prompt body measures 23,046 characters; the provider read reports about 22,658. Byte equality between the two is not established, so the provider prompt stays `PARTIALLY_SUPPORTED` (see `provider-snapshot-reconciliation.md`).

## 4. Voice / TTS

| Surface | Value | Status |
|---|---|---|
| TTS model | `eleven_v3_conversational` | `VERIFIED_SNAPSHOT` |
| Voice ID | `6u6JbqKdaQy89ENzLSju` | `VERIFIED_SNAPSHOT` |
| Expressive mode | `true` | `VERIFIED_SNAPSHOT` |
| Stability | `0.46` | `VERIFIED_SNAPSHOT` |
| Speed | `1.04` | `VERIFIED_SNAPSHOT` |
| Similarity boost | `0.8` | `VERIFIED_SNAPSHOT` |
| Style | not present in the read | `SOURCE_NEEDED` |
| Streaming latency optimization | `3` | `VERIFIED_SNAPSHOT` |
| Output audio | `pcm_16000` | `VERIFIED_SNAPSHOT` |
| Text normalisation | `system_prompt` | `VERIFIED_SNAPSHOT` |
| Phoneme tags | enabled | `VERIFIED_SNAPSHOT` |
| Audio effects | `null` | `VERIFIED_SNAPSHOT` |
| Suggested audio tags | `Selbstbewusst`, `Lacht`, `Geduldig` | `VERIFIED_SNAPSHOT` |
| Voice filter | dashboard-only in the read | `SOURCE_NEEDED` |

## 5. ASR and turn-taking

| Surface | Value | Status |
|---|---|---|
| ASR provider | `scribe_realtime` | `VERIFIED_SNAPSHOT` |
| ASR quality | `high` | `VERIFIED_SNAPSHOT` |
| Input audio | `pcm_16000` | `VERIFIED_SNAPSHOT` |
| ASR keywords | `[]` | `VERIFIED_SNAPSHOT` |
| Turn model | `turn_v3` | `VERIFIED_SNAPSHOT` |
| Turn timeout | `7s` | `VERIFIED_SNAPSHOT` |
| Turn eagerness | `normal` | `VERIFIED_SNAPSHOT` |
| Mode | `turn` | `VERIFIED_SNAPSHOT` |
| Spelling patience | `auto` | `VERIFIED_SNAPSHOT` |
| Speculative turn | `true` | `VERIFIED_SNAPSHOT` |
| Retranscribe on timeout | `false` | `VERIFIED_SNAPSHOT` |
| Silence end-call timeout | `-1` | `VERIFIED_SNAPSHOT` |
| Initial wait | `null` | `VERIFIED_SNAPSHOT` |
| Soft timeout | filler `Hhmmmm...yeah.` stored, `timeout_seconds=-1` | `VERIFIED_SNAPSHOT` (configured, not proven active) |
| Interruption sensitivity/thresholds | not present in the read | `SOURCE_NEEDED` |

## 6. Conversation surface

| Surface | Value | Status |
|---|---|---|
| Text only | `false` | `VERIFIED_SNAPSHOT` |
| Max duration | `600s` | `VERIFIED_SNAPSHOT` |
| Client events | audio, interruption, user_transcript, agent_response, agent_response_correction | `VERIFIED_SNAPSHOT` |
| Monitoring | `false` | `VERIFIED_SNAPSHOT` |
| Source attribution | `true` | `VERIFIED_SNAPSHOT` |
| DTMF | `null` | `VERIFIED_SNAPSHOT` |
| Compaction | no active values evidenced | `SOURCE_NEEDED` |
| Background voice detection | `false` | `VERIFIED_SNAPSHOT` |
| File input | `enabled=true`, max 10 files in memory, max 10 files per conversation | `VERIFIED_SNAPSHOT` / review required (PXK-6 security repair) |
| Audio environment | `source_type=null`, `source_id=null`, `volume=0.15`, `crossfade_loop=true` | `VERIFIED_SNAPSHOT`; audible background audio not evidenced |

## 7. Dynamic Variables

| Surface | Value | Status |
|---|---|---|
| Provider placeholders | 15: `company_name`, `company_website`, `prospect_name`, `prospect_salutation`, `call_compliance_status`, `call_compliance_note`, `do_not_contact`, `lead_source`, `consultant_name`, `meeting_duration_minutes`, `meeting_description`, `offer_process`, `website_analysis_report`, `agency_name`, `verified_finding` | `VERIFIED_SNAPSHOT` |
| Placeholder defaults | all empty | `VERIFIED_SNAPSHOT` |
| Runtime population path (batch/Twilio/API) | not verified | `SOURCE_NEEDED` |
| Shared project contract | v1.3 = 96 total / 95 custom DVs | `PARTIAL_VERIFIED_PROJECT_CONTRACT` |
| 15 provider vs. 95 contract variables | open contract drift; no ad-hoc expansion before classification | `OPEN_DECISION` |

## 8. Knowledge Base and RAG

| Surface | Value | Status |
|---|---|---|
| Bound KB resources | 8 (four Pixelkiez URL bindings incl. one second binding and one English page, Impressum URL, Datenschutzerklärung URL, folders `pixelkiez.de` and `pixelkiez.de/en Crawl Job (2026-08-25)`, file `pixelkiez_voice_agent_briefing.md`) | `VERIFIED_SNAPSHOT` |
| KB resource IDs / content digests | not captured | `SOURCE_NEEDED` |
| RAG enabled | `true` | `VERIFIED_SNAPSHOT` |
| Embedding model | `multilingual_e5_large_instruct` | `VERIFIED_SNAPSHOT` |
| Optional RAG | `false` | `VERIFIED_SNAPSHOT` |
| Max vector distance | `0.6` | `VERIFIED_SNAPSHOT` |
| Max documents length | `50000` | `VERIFIED_SNAPSHOT` |
| Max retrieved chunks | `20` | `VERIFIED_SNAPSHOT` |

## 9. Tools, workflow, MCP, Procedures

| Surface | Value | Status |
|---|---|---|
| Standalone tools | `prompt.tool_ids = []` | `VERIFIED_EMPTY_SNAPSHOT` |
| Legacy tools | `prompt.tools = []` | `VERIFIED_EMPTY_SNAPSHOT` |
| Built-in/system tools | all read built-ins `null` (`end_call`, `update_state`, `language_detection`, `transfer_to_agent`, `transfer_to_number`, `skip_turn`, `voicemail_detection`, `play_keypad_touch_tone`) | `VERIFIED_NULL_SNAPSHOT` |
| MCP bindings | `mcp_server_ids = []`, `native_mcp_server_ids = []` | `VERIFIED_EMPTY_SNAPSHOT` |
| Workflow | none found in the agent configuration | `VERIFIED_SNAPSHOT` |
| Procedures | the config read returns no reliable Procedure list | `SOURCE_NEEDED` (dedicated Procedure read) |

## 10. Guardrails, analysis, tests

| Surface | Value | Status |
|---|---|---|
| Guardrails enabled | `focus`, `prompt_injection` | `VERIFIED_SNAPSHOT` |
| Guardrail detail mode / thresholds / blocking | not in the read | `SOURCE_NEEDED` |
| Success Evaluations | `[]` | `VERIFIED_EMPTY_SNAPSHOT` |
| Data Collection | `[]` | `VERIFIED_EMPTY_SNAPSHOT` |
| Julia-specific provider tests | none identified in the global list; PXKEV 09 label `UNVERIFIED_EMPTY` | `SOURCE_NEEDED` (dedicated agent-test read) |

## 11. Widget, channels, telephony, security

| Surface | Value | Status |
|---|---|---|
| Widget config | `has_widget_config=true`; public deployment not implied | `VERIFIED_SNAPSHOT` |
| Phone number / Twilio / SIP binding | not derivable from the read | `SOURCE_NEEDED` |
| Inbound/outbound channel binding | not derivable from the read | `SOURCE_NEEDED` |
| Agent authentication / signed URLs | not derivable from the read | `SOURCE_NEEDED` |
| Allowlists | not derivable from the read | `SOURCE_NEEDED` |
| Override security flags / allowed runtime overrides | not derivable from the read | `SOURCE_NEEDED` |
| Privacy / retention | not derivable from the read | `SOURCE_NEEDED` |
| Recording | not derivable from the read | `SOURCE_NEEDED` |
| Agent/workspace call limits | not derivable from the read | `SOURCE_NEEDED` |

Missing visibility is never interpreted as `false` or disabled.

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

These are **prompt policy**, not proof that provider-level conversation-flow settings enforce the policy. The provider read shows 0 bound tools and 0 enabled built-ins, so action language in the prompt has no technical side-effect path.

## Completion gate for provider-exact baseline

The provider core (items 1–8 of the original gate, except the immutable prompt/First Message export and KB digests) is now snapshot-bound. The inventory stays `PARTIAL` until an immutable provider export/API read additionally covers:

1. an immutable raw export of System Prompt and First Message (byte-comparable with `prompt-baseline.md`);
2. Knowledge Base resource IDs and content digests;
3. interruption thresholds, voice style and voice filter;
4. Procedures (dedicated read);
5. Julia-specific provider tests (dedicated agent-test read) and, separately, actual run results;
6. guardrail detail mode/thresholds;
7. traffic allocation, telephony/channel binding, authentication, allowlists, overrides, retention, recording and call limits;
8. the runtime population path of the Dynamic Variables.

Until then, **provider-exact behavioral reproduction remains false** even though the prompt/policy baseline and the provider core are frozen.
