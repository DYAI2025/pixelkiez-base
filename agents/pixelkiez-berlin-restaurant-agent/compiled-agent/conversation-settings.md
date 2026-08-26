# Conversation Settings

Platform-level settings must be tuned in ElevenLabs and tested for this campaign. Current build config:

```json
{
  "status": "DRAFT_REQUIRES_ELEVENLABS_TUNING",
  "language": "de-DE",
  "tone": "kurz, sachlich, freundlich, nicht draengend",
  "turn_policy": "eine Hauptfrage pro Turn; keine langen Audit-Monologe",
  "restaurant_context": "Stoerungen im Servicebetrieb minimieren; Busy-Signal sofort respektieren",
  "recording": "OFF"
}
```

Do not encode timing/interruption mechanics as unsupported psychological prompt rules.
