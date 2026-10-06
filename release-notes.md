# DictaText 0.7.1

- Dark dashboard with compact sidebar, original identity, real insights and daily radial activity.
- Local usage analytics by category and executable; old records remain unclassified. No dictation content is read for analytics.
- Large preferences window, per-change confirmation, application classification, installation and encrypted data location in About.
- Explicit GitHub Releases updater: stable SemVer, verified manifest, SHA-256, signature validation when signed, isolated helper, binary backup/rollback and exact installation destination.
- Updates preserve personal data and existing valid LLM/speech models; no LLM GGUF is bundled.

Physical QA of dictation, microphone changes and appearance remains required. This release does not assert that DictaText V1 is finished or that previously reported lexical ASR errors are resolved. No RNNoise filter has been added without A/B evidence.

Cancellation fix: closing the update offer has one cancellation path, asynchronous decision continuations and a lifecycle guard. Release 0.7.0 was withdrawn after the final physical UI check exposed this race.

Verified source commit: 834515006c90616f664e78bed79858d137923a0a
Tests: 412/412; installed/native/updater integration PASS.
